# Building the system page with the DesignA11y system
## Workflow validation report · October 18, 2026

**Owner:** Dana Randall  
**Assessment:** Partially delivered. Useful implementation case study; no controlled performance claim.  
**Live page:** https://www.design-a11y.com/design-system

The system helped carry documented brand, content and accessibility intent into a real Squarespace page. It provided usable decisions about hierarchy, color roles, focus, targets, motion and responsive composition. It did not yet provide a mapped production component library, automatic synchronization, or complete validation. The strongest result is traceability: we can identify the source of a requirement, inspect its implementation and record the gaps.

The page is a published working resource. The Figma Community release remains planned. Publishing this page is not a declaration that the system or site meets every accessibility requirement.

## 1. What we built

- A resource page explaining the system, its foundations, four-source workflow, testing approach and current build status.
- A **System** main-navigation destination at /design-system. Published order: Toolkit, Resources, System, Articles.
- A homepage feature after Latest perspectives and before signup, preserving the established article/toolkit hierarchy.
- A Resources promo alongside the Toolkit, using two equal-width cards that stack on narrow screens.
- Equal-height resource cards on the system page, without fixed text heights or line clamping.
- A reusable native FeaturedResourcePair family in Figma, plus an implementation Spec and versioned Squarespace source.

The page uses Anton headings and the existing live-site Proxima Nova. Archivo remains the approved Figma-system counterpart. Original sensory artwork and frame expression were retained. Motion Lab was excluded as a layout reference, and no Prime assets were redistributed.

## 2. The article’s promises, compared with the evidence

The reference article is [Figma Specs: Put Accessibility Into the Instructions Agents Build From](https://www.design-a11y.com/articles/figma-specs-accessibility-design-systems). It proposes a workflow and a future comparison; it does not establish that Specs already improve results.

| Proposed capability | What happened in this build | Assessment |
|---|---|---|
| Establish platform, foundations and source authority first | Read the foundational native Spec, Resources Spec, component focus contract and full toolkit references. Identified Squarespace and the intentional typography mapping. | Delivered for this task. |
| Give tokens intended roles and approved use | Applied Aubergine, Petal and Blush by purpose; checked the visible text pairs, including Rose/Copper swatch labels. Page CSS defines an explicit semantic adapter. | Delivered locally; no automated token export pipeline was demonstrated. |
| Retrieve full guidance at the time of work | Native Spec retrieval succeeded; full task references were read rather than using the condensed Figma skill as a substitute. | Retrieval demonstrated. Automatic routing from the condensed skill was not tested. |
| Give components behavioral contracts | Used documented anchor semantics, 44px targets, static focus, finite hover feedback, responsive stacking and decorative-image purpose. | Useful instructions; they still required deliberate implementation. |
| Reuse implemented components | Reused the native Squarespace shell and translated compatible Figma patterns into semantic HTML/CSS. No mapped production component library or Code Connect implementation existed. | Partial. This was design-pattern reuse, not proven code-component reuse. |
| Specify composition and the experience between sections | Added logical headings, named topic navigation, stable target IDs, immediate scrolling and meaningful resource links. | Delivered for a primarily editorial page. Complex forms/dialogs were not exercised. |
| Validate the implementation against observable requirements | Inspected the actual rendered page, contrast pairs, target geometry, focus and mobile menu behavior. Attempted the toolkit’s two named engine families. | Partial: direct live-route scans were blocked; captured-DOM checks and a manual queue remain separate evidence. |
| Feed discoveries back into the system | Added a native implementation Spec, the paired-promo family, source files, report, machine mapping and review queue; reconciled navigation guidance. | Delivered as an explicit maintenance step, not automatic synchronization. |
| Show that fuller Specs outperform the condensed skill | No independent control arm, pre-registered scoring rubric, repeated trials or comparable timing/cost data. | Not tested. No causal or efficiency claim is supported. |

## 3. Findings and attribution

A visitor experiences a barrier regardless of its source. Attribution identifies where to fix and maintain it; it is not an exemption.

| Finding | Origin supported by the evidence | Action / remaining work |
|---|---|---|
| Design components lacked production mappings | System maturity gap | Recorded the missing code library/Code Connect layer. Committed the actual adapter as a concrete reuse target. |
| Proposed WEB token names were not already production CSS | System-to-platform integration gap | Defined semantic page-level properties. Do not describe this as automatic export or token synchronization. |
| Inherited smooth scrolling moved the viewport during keyboard traversal | Existing site integration; not established as a Squarespace product defect | Set immediate scrolling for the system page. |
| Shared header/footer links fell below the 44px house standard | Existing shell geometry/content styling, outside the new content components | Added page-scoped target-size support. This is a house-standard finding, not by itself proof of a WCAG 2.5.8 failure. |
| Native burger button changed name but lacked aria-expanded/aria-controls | Observed Squarespace-emitted menu markup on this site | Added a scoped adapter that follows the native menu-open class. Retained native opening, Escape and focus return. Regression-test after platform updates. |
| Homepage inverse promo inherited dark text on its dark background | Consuming-code CSS cascade mistake | Corrected the scoped foreground rules; rechecked Petal text on Aubergine. Do not attribute this to the toolkit or platform without evidence. |
| Two full-width resource promos used excessive space | Composition decision, identified by Dana | Changed to a paired desktop pattern and added the native Figma family. |
| Resource cards had unequal heights | Consuming layout implementation, identified by Dana | Used equal grid rows and flexible growing links. Preserved intentional hover lift. |
| Footer “Explore” and “Connect” are paragraph/strong markup | Existing authored footer semantics in the platform shell | Retained in the manual queue. Native heading/nav-group remediation should preserve visual style and be reviewed across the whole site. It is not a demonstrated platform limitation. |
| Direct engine runs could not reach the public host | Validation environment/connectivity | Logged the blocked run. Do not treat it as a clean scan or blame the system. |
| An early capture omitted description targets and geometry | Test-harness/export defect | Rejected that capture’s apparent violations as live-page evidence; repaired the capture to include the body and geometry, then reran. No engine rules were disabled. |
| A 320px measurement showed 1px document overflow | Small shell/hidden-content boundary, cause not fully established | No meaningful page-content clipping was observed. Keep a specific narrow reflow check open rather than declaring perfect reflow. |

The menu workaround adds metadata to the existing control. It does not replace native behavior, add an accessibility overlay, or claim to repair every Squarespace menu issue. Its class/selector dependency is now part of the maintenance contract.

## 4. Evidence collected

### Actual public page

The intended content loaded: **5,469 characters** in the page resource root. The page has one h1, the native main landmark, logical h2/h3 sections, an English document language and a descriptive page title. The hero artwork is decorative, has empty alt and is excluded from the accessibility tree.

Live checks covered:
- Resting visible text colors, descriptive anchors and resolved aria-describedby references.
- Page-content and scoped shell target sizes after repair.
- Wide composition and a verified 320 CSS px layout.
- Skip-link activation, visible focus and sequential keyboard access to page links.
- Mobile menu link order; Enter opening; Escape dismissal and focus return.
- Menu metadata changing false → true → false with native state.
- Equal card heights after the layout correction.

Measured text pairs in the page’s resting state:

| Foreground / background | Contrast |
|---|---:|
| Aubergine / Petal, and reverse | 11.91:1 |
| Aubergine / Blush, and reverse | 9.87:1 |
| Aubergine / Rose | 5.55:1 |
| Aubergine / Copper | 6.67:1 |

These values do not certify every component, theme, interaction state or image treatment. No text is placed over the decorative hero image.

### Automated checks: state exactly what ran

Installed **IBM accessibility-checker 4.0.34** and **Pa11y 10.0.0 / HTML_CodeSniffer**. IBM used the IBM_Accessibility policy with violation and potentialviolation fail levels, and manual/recommendation reporting retained.

**Live-route engine scans completed: 0.** Connectivity prevented the execution environment from loading the host. The public page was independently verified in the connected browser.

**Captured-DOM checks completed: 2 viewport captures × 2 engine families.** These are the final desktop and 320px resting-state exports, not live-route or interactive-state engine scans.

| Captured state | IBM | Pa11y / HTML_CodeSniffer |
|---|---|---|
| Desktop, 1380px | 0 definite violations; 16 potential violations; 1 recommendation; 1 manual item | 0 errors; 366 warnings; 72 notices |
| Narrow, 320px | 0 definite violations; 11 potential violations; 1 recommendation; 1 manual item | 0 errors; 367 warnings; 72 notices |

**IBM returned a non-passing status because potential violations remain.** Do not report either row simply as “passed.”

Captures serialize computed styles. They do not preserve actual web fonts, pseudo-elements, interactive listeners, or responsive/preference rules as executable behavior. Geometry was included, but this is still an exported representation. Pa11y’s many inherited-background warnings are strongly affected by that inline-style export; they are not 366 confirmed live defects. Every warning family and every IBM review item is retained in the evidence/queue.

IBM review families include focus visibility/obscuring, color independence, high-contrast behavior and footer heading intent. Pa11y also flags fixed positioning, footer headings, image/link meaning, text resizing, reflow, spacing, preferences and other manual conditions. A redundant native main role is a recommendation in Squarespace’s shell.

## 5. What this test did not establish

- Screen-reader announcement quality or usability for disabled people.
- Full 200%/400% zoom, text-only resizing or text-spacing override behavior.
- Actual OS reduced-motion, reduced-transparency and Windows forced-colors behavior.
- Production behavior for the library’s forms, tabs, dialogs, comboboxes or other complex widgets.
- Public Community duplication, variable/Spec transfer, licensing readiness or release completeness.
- Faster or cheaper agent execution, better accessibility than a control, or automatic reliable retrieval.
- A complete live-host automated scan or accessibility conformance.

The new page has no autonomous motion or particle initialization. Card movement is guarded by no-preference and fine-hover capability, with a static alternative. Source inspection is not a substitute for preference-setting tests.

## 6. What to improve next

1. **Provide production reuse targets.** Map the actual HTML/CSS/Squarespace adapters to the design components; add Code Connect where supported. Keep complex controls on tested primitives.
2. **Make contract retrieval repeatable.** Add an entry manifest with exact IDs, revisions, implementation paths and acceptance checks. Test it with an agent that did not help author the system.
3. **Automate drift detection.** Compare native APIs, Spec mirrors, token exports and component mappings. This build exposed the cost of explicit manual reconciliation.
4. **Create a Squarespace adapter contract.** Document safe selectors, ownership, regression checks and the boundary between platform markup, authored content and custom scripts.
5. **Complete live validation.** Run the two engines where they can load the real host and its menu-open state; work the human/AT queue and retain unresolved findings.
6. **Run the article’s actual comparison.** Use the same brief and criteria for the condensed skill and fuller-Spec workflow, record retrieval and output evidence, repeat tasks, and compare accessibility, effort and failure modes.

## 7. Source and artifact record

- Foundational native Spec: 12:2.
- Resources native Spec: 96:1063.
- Implementation native Spec: 108:1116.
- Retrieved Hero context: 87:8; approved focus: 17:7.
- Paired featured resource family: 106:1103.
- Full toolkit routing skill blob: 4e9b0e22f41f8f564c5bc3e1699ba7ba4389b09e.
- Toolkit references: agent-directives, html-css, testing, content-and-language, motion-media-targets, color.
- Task source and evidence: [page Spec](../specs/system-resource-page.md), [manual testing queue](../accessibility/MANUAL-TESTING.md), [machine contract](../../contracts/pages/system-resource.json).
- Raw captured-scan findings are retained privately in the working evidence package; this public report summarizes results. They are not live-route scan results.

**Conclusion:** The workflow made consequential intent available and useful. This page demonstrates that connection in practice. It also shows that documentation does not supply implementation, synchronization or proof. Those connections are the next part of the system to build.
