# System resource page — implementation contract

Contract ID: da.page.system-resource.v1
Owner: Dana Randall
Version: 0.1 · October 18, 2026
Runtime: Squarespace 7.1, native shared header/footer, one semantic HTML/CSS code block
URL: https://www.design-a11y.com/design-system
Source: site/squarespace/design-system-page.html in https://github.com/danarandall/designa11y-design-system

## Purpose and source authority

Explain the DesignA11y design system, its human and machine guidance, current availability and proposed workflow. This is an authentic resource page and a practical implementation case study. It is not a controlled comparison or evidence that Specs improve agent performance.

Apply the full AI A11y Toolkit and Dana's approved inclusive-design/AI context. Reuse compatible native design patterns; do not imply that design instances are runtime code components. No Code Connect production mapping existed for this build. Existing Squarespace navigation and typography remain the platform implementation.

Retrieved native Specs: 12:2 (foundation) and 96:1063 (Resources patterns). Retrieved Hero design context: 87:8. Git component focus contract: contracts/components/actions-and-fields.json. Toolkit routing skill and agent-directives, html-css, testing, content-and-language, motion-media-targets and color references were read. Native type mapping: Anton headings, Archivo in Figma, existing Proxima Nova in Squarespace. Motion Lab layout is excluded.

## Anatomy and semantics

One page h1: Designed for people. Defined for AI.
Reading order: editorial hero, purpose panel, named topic navigation, foundations, four-source workflow, testing explanation, resource grid, working status, feedback link.
Use actual h2/h3 headings, lists and anchors. Native Squarespace supplies the single main landmark, shared header/footer and skip link. Decorative hero surface/frame has empty alt and is excluded from assistive technology. Resource links use descriptive visible labels; no fake controls or nested interactive content.

System page resource grid: equal-height cards using grid-auto-rows:1fr, flexible list items and growing card links. No fixed text heights or line clamping.
Resources page featured pair: Toolkit and Design System in two equal columns above topic navigation; stack at <=767px. Native family Resources/FeaturedResourcePair 106:1103, Wide 106:1065 and Stacked 106:1084. Nested panels preserve Title, Body, CTA and Verification note APIs.
Homepage: inverse editorial feature after Latest perspectives and before signup. Preserve existing graphics and article/toolkit hierarchy.
Shared main navigation: Toolkit, Resources, System, Articles. System links to /design-system. Native Header 59:160 mirrors this order.

## Tokens and behavior

Use Aubergine text on Petal/Blush; Petal text on Aubergine; Rose and Copper are named swatches and accents. Measured visible text pairs range 5.55:1 to 11.91:1 in this page's reviewed resting state.
44x44 CSS px house targets; anchors and buttons grow with labels. Heading sizes use responsive formulas and content wraps.
Page-content links implement static 17:7 focus: three square 2px bands, 5px gap, 11px outset; pearl band uses the approved gradient. Shared shell gets a scoped three-band fallback and system-color forced-colors outline.
Card hover: -3px / 140ms ease-out only with no reduced-motion request and a fine hover pointer. No page-load animation, particle initialization or looping effects. Focus does not move the card.
Topic jumps use stable IDs, 160px scroll margin and immediate scrolling on this page.

## Squarespace adapter boundary

The source includes page-scoped integration CSS for shared link target size, focus and a visually hidden external-link notice. It does not globally redesign the site.
Native burger button received a scoped metadata adapter: aria-controls references the existing mobile navigation; aria-expanded follows the native body header--menu-open class. Native opening, Escape handling and focus return are preserved. The adapter observes body class changes and disconnects on pagehide; it is not a replacement menu or accessibility overlay.
This selector/class dependency requires regression checks after Squarespace updates. Missing state was observed in emitted platform markup; smooth scrolling and inherited color/focus styles were existing site integration, not established Squarespace product defects.

## Validation and evidence boundaries

Live browser: page title/language/landmarks, content-loaded assertion (5,469 characters), heading hierarchy, image purpose, resting contrast, targets, desktop geometry, 320px reflow, links, skip link, focus, mobile menu order/keyboard/Escape and expanded-state synchronization were inspected.
Static DOM captures were scanned separately with IBM Equal Access and Pa11y/HTML_CodeSniffer. Captures serialize computed styles and lose native fonts, interactive listeners, pseudo-elements and responsive rules; their counts cannot be presented as live-route passes. Direct live-route scans were blocked by environment connectivity.
Queue human review for screen-reader announcements, sense of reading/focus order, image purpose, copy clarity, text-only resizing, 200%/400% zoom, spacing overrides, preference settings and Windows forced colors. Keep raw findings and platform versus implementation attribution. No conformance or performance certification.

Community release remains planned; do not present the working Figma file as a published Community resource. Prime reference material must not be redistributed.
