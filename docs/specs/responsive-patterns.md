# Responsive application patterns

Contract ID: da.patterns.v1 Owner: Dana Randall · October 18, 2026 Status: native component drafts; production behavior unimplemented/unvalidated

Working compositions built from native system instances. These are architecture and reflow drafts, not a replacement homepage design or a claim that the live site was changed.

## Patterns/Homepage

ID: da.patterns.home

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=68-110)

Purpose: Editorial homepage hierarchy with toolkit prominence and distinct featured/latest content.

States: Desktop, Mobile. Text properties: Headline, Introduction.

Semantics: Header, main, labelled sections and footer; one h1; meaningful article links and reading order.

Keyboard: Skip link first; consistent nav and card order; no duplicate featured story in next block.

Motion: contracts/motion/interface-microinteractions.json

## Patterns/Article

ID: da.patterns.article

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=68-149)

Purpose: Long-form article template with author, metadata and related resources.

States: Desktop, Mobile. Text properties: Title.

Semantics: Article landmark, one h1, publication time, byline and logical heading hierarchy.

Keyboard: In-page links and related resources follow document order; skip repetitive navigation.

Motion: contracts/motion/interface-microinteractions.json

## Patterns/ToolkitLanding

ID: da.patterns.toolkit

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=68-184)

Purpose: Route people to practical design, engineering and content guidance.

States: Desktop, Mobile. Text properties: Title, Introduction.

Semantics: Main heading, introductory guidance and linked resource groups; revision provenance explicit.

Keyboard: Clear headings and links; no hidden essential guidance.

Motion: contracts/motion/interface-microinteractions.json

## Patterns/SearchResults

ID: da.patterns.results

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=68-239)

Purpose: Search context, result count, filters and recovery.

States: Results, Empty, Loading. Text properties: .

Semantics: Search landmark and main results region; polite result status; filters have labels.

Keyboard: Search does not steal focus on result update; pagination preserves predictable navigation.

Motion: contracts/motion/interface-microinteractions.json

## Patterns/PreferencesForm

ID: da.patterns.form

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=68-278)

Purpose: Compose labelled form controls, help, validation and outcomes.

States: Default, Error, Success. Text properties: .

Semantics: Native form with grouped controls, error summary and associated inline messages; preserve entered values.

Keyboard: Submit validates; focus summary or first invalid according to flow; success status without unexpected focus change.

Motion: contracts/motion/interface-microinteractions.json

## Patterns/MotionLab

ID: da.patterns.motion-lab

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=68-303)

Purpose: Demonstrate and evaluate reusable production-interface microinteractions.

States: Ready, StaticAlternative. Text properties: .

Semantics: Named demo sections with instructions, explicit replay/pause where required and static alternatives. No live-site demo inventory claimed.

Keyboard: Named controls operate by keyboard/touch; repeated animation is user initiated; preserve focus and alternative feedback.

Motion: contracts/motion/interface-microinteractions.json

## Shared anatomy, tokens and layout

Semantic surface, text, action and border variables; shared Archivo type styles; space metrics and square radii. Named native layers and public text properties. Focus uses component 17:7, static triple stroke with 11px outset and 5px clear gap; never clip. Text wraps and height grows. Example widths are documentation examples, not fixed production widths. Intrinsic icons, grids and media proportions are intentional geometry.

## Implementation and evidence

Use native controls and tested headless primitives for complex patterns. Full AI A11y Toolkit reference/design.md is authoritative. Never treat drawings as keyboard or ARIA implementations. Do not improvise complex controls from these vectors. Implementation mapping: unassigned.

Before release: verify light/dark pairings and forced colors, keyboard/focus/announcements, 44px targets, 320px reflow and enlarged text, touch parity, interruption and reduced-motion alternatives, loading/error states and human review with named browser/AT pairings. Record evidence per component.

No Prime artwork, licensed components or code copied. Prime informed category breadth only. Existing live-site use is not a prerequisite for system inclusion.

<!-- Figma source: https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=68-456 · mirrored October 18, 2026 -->
