# System page — manual testing and unresolved items

Added: October 18, 2026
Owner: Dana Randall
Page: https://www.design-a11y.com/design-system
Implementation: site/squarespace/design-system-page.html

The live browser checks in the report are observations, not human or assistive-technology sign-off. Leave human results blank until a named tester records the pairing, date and result. Do not suppress engine findings.

| ID | Why review / related criteria | How to test | Expected result | Human result |
|---|---|---|---|---|
| M01 | Reading order and heading meaning · 1.3.1, 2.4.6 | Read the page by headings and in document order with a screen reader. | One clear h1; purpose, foundations, workflow, test, resources and status form a coherent sequence. | |
| M02 | Skip link and focus visibility · 2.4.1, 2.4.7, 2.4.11 | Start at page top, Tab, activate Skip to Content, then continue through every link. | Skip appears; repeated navigation is bypassed; focus is visible and unobscured. | |
| M03 | IBM potential focus-obscuring items · 2.4.11 | Tab to logo, primary links, contract links and resource cards at wide/narrow widths and enlarged text. Scroll as needed without moving focus. | Focus can be located and is not hidden behind sticky UI or cropped rings. | |
| M04 | Native mobile menu with scoped adapter · 4.1.2, 2.1.1 | At 320px, open menu with Enter/Space; read the button state; Tab links; Escape. | Announces expanded state; Toolkit, Resources, System, Articles order; closes and returns focus to trigger. | |
| M05 | Link purpose and label-in-name · 2.4.4, 2.5.3 | Review a links list and activate visible labels with voice control. | Names identify destinations; external-tab notice is meaningful and does not replace the visible name. | |
| M06 | Decorative image and wordmarks · 1.1.1 | Review the hero and home links with a screen reader. | Decorative surface/frame is skipped; wordmark home links have a useful name without repetition. | |
| M07 | Text enlargement and spacing · 1.4.4, 1.4.10, 1.4.12 | Test 200% and 400% page zoom, Firefox text-only zoom, larger default text and WCAG text-spacing overrides. | No text loss, overlap, clipping, unreachable links or fixed-height truncation. | |
| M08 | Narrow reflow boundary · 1.4.10 | At 320 CSS px inspect full page and both promo locations. Test long labels. Investigate the measured 1px document overflow. | Content remains in one vertical flow; overflow does not hide meaningful content or require horizontal reading. | |
| M09 | Forced colors and IBM manual high-contrast item · 1.4.11 | Test Windows High Contrast/forced colors with keyboard focus. | Text/links remain distinguishable; system focus outline remains visible; decorative effects are unnecessary. | |
| M10 | Motion preferences · 2.2.2, sensory review | Enable reduced motion, then load and hover the cards. Repeat with a coarse pointer and without the preference. | Reduced/coarse paths are static; fine-pointer motion is finite -3px/140ms only on the acted-on card; no page-load or looping motion. | |
| M11 | Color independence · 1.4.1 | Review in grayscale and with representative color-vision simulations. | Swatches retain names; hierarchy and links do not rely on color alone. | |
| M12 | Increased contrast / reduced transparency | Enable relevant OS/browser settings and reload. | Decorative masking/transparency can disappear without losing content or meaning. | |
| M13 | Plain language and workflow claims | Ask designers and builders unfamiliar with the project to explain what is available now and how the workflow works. | Understand working versus released status; no implication of automatic accessibility or proven performance. | |
| M14 | Resources/homepage integration | Review desktop paired promos, mobile stacking and the homepage feature after Latest perspectives. Follow each system link. | Two clear resources; coherent placement; readable inverse foreground; /design-system destination works. | |
| M15 | Blocked live-route engine scan | Run IBM Equal Access with IBM_Accessibility and Pa11y/HTML_CodeSniffer where the real host is reachable; scan resting and menu-open states after asserting real content. | Preserve all findings and rendered counts; repair/triage before calling the live scan complete. | |

Suggested pairings: VoiceOver + Safari on macOS/iOS, NVDA + Firefox or Chrome on Windows, TalkBack + Chrome on Android. Include disabled participants using their own settings and record which pairing finds each issue.

## Unresolved / attribution

- **Existing authored footer:** Explore and Connect are paragraph/strong labels. IBM text_block_heading and Pa11y H42 request semantic review. Decide whether to use real headings and separately named navigation groups in the shared footer; retain visual styling. This is not established as a Squarespace limitation.
- **Squarespace shell recommendation:** aria_role_redundant on native main. Native main already supplies the correct landmark; redundant role is not a definite failure. Record before changing platform output.
- **Platform regression:** the page-scoped menu-state adapter depends on .header-burger-btn, .header-menu-nav-list and body.header--menu-open. Re-test after Squarespace updates.
- **Direct live-host engine coverage:** blocked by connectivity. Captured-DOM results cannot close this.
- **Native Figma/runtime parity:** drawings, code, public properties and Specs require explicit reconciliation; Code Connect remains unmapped.

## Engine review-item inventory

Final captured desktop IBM: 16 potential violations, 1 recommendation, 1 manual; final captured narrow IBM: 11 potential violations, 1 recommendation, 1 manual. No definite violations were reported in those captures. IBM returned non-pass because potential items remain.

- style_highcontrast_visible → M09.
- style_color_misuse → M11.
- element_tabbable_visible → M02.
- element_tabbable_unobscured → M03.
- text_block_heading → footer review above; the brand tagline is prose, while Explore/Connect organize links.
- aria_role_redundant → native-main recommendation above.

Pa11y desktop: 366 warnings, 72 notices; narrow: 367 warnings, 72 notices, no errors. All warning families retained: 360 inherited-background warnings per capture, three fixed-position warnings, two heading warnings, and one desktop/two narrow absolute-background warnings. Inline computed-style export strongly affects these warnings; inspect actual backgrounds and geometry, not the count alone. The full notice set is retained in the evidence package and mapped by topic to M01–M15.
