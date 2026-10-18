# Structured data and resource lists

Contract ID: da.data.v1 Owner: Dana Randall · October 18, 2026 Status: native component drafts; production behavior unimplemented/unvalidated

Readable structured information with explicit relationships, sorting and filtering. Use semantic tables and lists; opt into a tested data-grid implementation only when interaction requires it.

## Data/TableCell

ID: da.data.table-cell

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=64-11)

Purpose: Consistent table cell anatomy and content alignment.

States: Header, Text, Numeric, Status. Text properties: Content.

Semantics: th with scope for headers; td for data; numeric values preserve units; statuses explicit text.

Keyboard: Cells are not tab stops in plain tables; only interactive descendants.

Motion: contracts/motion/interface-microinteractions.json

## Data/Table

ID: da.data.table

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=64-117)

Purpose: Compare structured resource information without sacrificing reading order.

States: Default, Sorted, RowSelected, Loading, Empty, Compact. Text properties: Caption.

Semantics: Native table with caption and scoped headers. Sort buttons expose aria-sort. Row selection uses named checkboxes. Data grid only with full tested grid behavior.

Keyboard: Normal tab order through sorting/actions/checkboxes; horizontal scroll keyboard-accessible if needed; do not add grid arrows to static tables.

Motion: contracts/motion/interface-microinteractions.json

## Data/DescriptionList

ID: da.data.description-list

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=64-138)

Purpose: Present labelled resource or system metadata.

States: Stacked, Inline. Text properties: .

Semantics: Native dl/dt/dd for name/value relationships; do not substitute a table for unrelated facts.

Keyboard: Static text; link values behave normally.

Motion: contracts/motion/interface-microinteractions.json

## Data/FilterBar

ID: da.data.filter-bar

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=64-157)

Purpose: Filter content with clear scope and reversible choices.

States: Default, FiltersApplied, NoResults. Text properties: Title, Result count.

Semantics: Labelled form/group with native controls, result count status and reset action.

Keyboard: Tab to controls; Enter submits when applicable; removing filters announces result changes without stealing focus.

Motion: contracts/motion/interface-microinteractions.json

## Data/ResourceList

ID: da.data.list

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=64-175)

Purpose: Compose accessible resource list items with stable ordering.

States: Default, Loading, Empty. Text properties: Title.

Semantics: Native list and labelled items; status separate from item names.

Keyboard: Normal link order; loading does not remove focused content.

Motion: contracts/motion/interface-microinteractions.json

## Shared anatomy, tokens and layout

Semantic surface, text, action and border variables; shared Archivo type styles; space metrics and square radii. Named native layers and public text properties. Focus uses component 17:7, static triple stroke with 11px outset and 5px clear gap; never clip. Text wraps and height grows. Example widths are documentation examples, not fixed production widths. Intrinsic icons, grids and media proportions are intentional geometry.

## Implementation and evidence

Use native controls and tested headless primitives for complex patterns. Full AI A11y Toolkit reference/design.md is authoritative. Never treat drawings as keyboard or ARIA implementations. Do not improvise complex controls from these vectors. Implementation mapping: unassigned.

Before release: verify light/dark pairings and forced colors, keyboard/focus/announcements, 44px targets, 320px reflow and enlarged text, touch parity, interruption and reduced-motion alternatives, loading/error states and human review with named browser/AT pairings. Record evidence per component.

No Prime artwork, licensed components or code copied. Prime informed category breadth only. Existing live-site use is not a prerequisite for system inclusion.

<!-- Figma source: https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=64-245 · mirrored October 18, 2026 -->
