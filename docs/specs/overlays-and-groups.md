# Overlays and grouped actions

Contract ID: da.overlays.v1 Owner: Dana Randall · October 18, 2026 Status: native component drafts; production behavior unimplemented/unvalidated

Bounded contextual tasks, explicit choices and intentional focus management. Actions reuse the native DesignA11y button components. Drawings require tested runtime primitives before release.

## Overlays/Dialog

ID: da.overlays.dialog

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=63-25)

Purpose: Focus a bounded task requiring an explicit response.

States: Information, Confirmation, FormError. Text properties: Body. Heading follows the semantic state.

Semantics: Tested modal dialog primitive or native dialog; labelled by heading; background inert; nonmodal remains distinct.

Keyboard: Initial focus intentional; Tab trapped inside modal; Escape closes when safe; restore invoking control focus.

Motion: contracts/motion/interface-microinteractions.json

## Overlays/Drawer

ID: da.overlays.drawer

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=63-50)

Purpose: Offer contextual detail or filters without losing the underlying task.

States: Details, Filters, Mobile. Text properties: Body. Heading follows the semantic state.

Semantics: Modal drawer uses dialog primitive; persistent desktop panel is an aside, not a focus trap.

Keyboard: Modal Tab containment/Escape/return focus; persistent panel follows document order.

Motion: contracts/motion/interface-microinteractions.json

## Overlays/Popover

ID: da.overlays.popover

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=63-59)

Purpose: Show a small contextual surface tied to a trigger.

States: Information, Actions. Text properties: Title, Body.

Semantics: Tested nonmodal popover; role based on content, not automatic tooltip/menu. Trigger expanded and controls where appropriate.

Keyboard: Trigger Enter/Space; content reachable logically; Escape dismisses and restores focus if it moved.

Motion: contracts/motion/interface-microinteractions.json

## Overlays/PreferenceBanner

ID: da.overlays.banner

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=63-74)

Purpose: Give clear optional preference choices without coercion.

States: Consent, Preferences. Text properties: Title, Body.

Semantics: Named region with equivalent accept/reject or preference controls; no preselected optional consent.

Keyboard: Logical controls; no focus trap unless intentionally modal; no disappearing time limit.

Motion: contracts/motion/interface-microinteractions.json

## Actions/ButtonGroup

ID: da.actions.button-group

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=63-86)

Purpose: Group related actions with clear primary hierarchy.

States: Horizontal, Stacked. Text properties: .

Semantics: Named group only when helpful; native buttons and links retain their semantics.

Keyboard: Normal Tab order; use toolbar roving model only when intentionally implementing toolbar.

Motion: contracts/motion/interface-microinteractions.json

## Actions/SegmentedControl

ID: da.actions.segmented-control

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=63-115)

Purpose: Choose a single compact view or mode.

States: FirstSelected, SecondSelected, Focus. Text properties: .

Semantics: Radio group for a setting; tabs only when controlling associated panels; do not mix roles.

Keyboard: Radio-group arrows and Space, or tabs model when used as tabs; specify consuming intent.

Motion: contracts/motion/interface-microinteractions.json

## Shared anatomy, tokens and layout

Semantic surface, text, action and border variables; shared Archivo type styles; space metrics and square radii. Named native layers and public text properties. Focus uses component 17:7, static triple stroke with 11px outset and 5px clear gap; never clip. Text wraps and height grows. Example widths are documentation examples, not fixed production widths. Intrinsic icons, grids and media proportions are intentional geometry.

## Implementation and evidence

Use native controls and tested headless primitives for complex patterns. Full AI A11y Toolkit reference/design.md is authoritative. Never treat drawings as keyboard or ARIA implementations. Do not improvise complex controls from these vectors. Implementation mapping: unassigned.

Before release: verify light/dark pairings and forced colors, keyboard/focus/announcements, 44px targets, 320px reflow and enlarged text, touch parity, interruption and reduced-motion alternatives, loading/error states and human review with named browser/AT pairings. Record evidence per component.

No Prime artwork, licensed components or code copied. Prime informed category breadth only. Existing live-site use is not a prerequisite for system inclusion.
