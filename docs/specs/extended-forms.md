# Extended form controls

Contract ID: da.forms.extended.v1 Owner: Dana Randall · October 18, 2026 Status: native component drafts; production behavior unimplemented/unvalidated

Original extended form controls. Native browser controls and tested behavior primitives are required in implementation.

## Forms/Select

ID: da.forms.select

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=58-179)

Purpose: Select one topic from a finite list.

States: Default, Hover, Focus, Disabled, Error. Text properties: Label, Value, Helper text.

Semantics: Native select with associated visible label; browser popup.

Keyboard: Native select keys and typeahead; Tab exits.

Motion: contracts/motion/interface-microinteractions.json

## Forms/Combobox

ID: da.forms.combobox

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=58-232)

Purpose: Find a resource in a longer option set.

States: Default, Focus, Expanded, Empty, Error, Disabled. Text properties: Label, Value, Helper text.

Semantics: Tested combobox primitive with expanded/controls/active-descendant; named listbox and options.

Keyboard: Arrows navigate, Enter selects, Escape closes; preserve editing keys.

Motion: contracts/motion/interface-microinteractions.json

## Forms/Search

ID: da.forms.search

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=58-273)

Purpose: Search DesignA11y articles and resources.

States: Default, Focus, Loading, Error. Text properties: Label, Value, Helper text.

Semantics: Native search input in labelled search form; result status on submit.

Keyboard: Enter submits; native editing and named clear control.

Motion: contracts/motion/interface-microinteractions.json

## Forms/DateField

ID: da.forms.date-field

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=58-306)

Purpose: Enter a date with clear format and calendar alternative.

States: Default, Focus, Error, Disabled. Text properties: Label, Value, Helper text.

Semantics: Native date input or tested date field; associated label and format help.

Keyboard: Native editing; no blocked manual entry; named calendar trigger.

Motion: contracts/motion/interface-microinteractions.json

## Forms/FileUpload

ID: da.forms.file-upload

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=58-337)

Purpose: Attach supporting material with explicit constraints.

States: Default, Selected, Error, Disabled. Text properties: Label.

Semantics: Native file input with visible label; drag/drop is supplemental.

Keyboard: Keyboard file chooser; separately named remove action; selection status.

Motion: contracts/motion/interface-microinteractions.json

## Forms/Slider

ID: da.forms.slider

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=58-363)

Purpose: Adjust a bounded value with numeric entry available.

States: Default, Focus, Disabled. Text properties: Label, Value text.

Semantics: Native range input or tested slider; name, min/max/value and value text; numeric alternative.

Keyboard: Arrows step, Home/End reach bounds.

Motion: contracts/motion/interface-microinteractions.json

## Forms/NumberStepper

ID: da.forms.stepper

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=58-393)

Purpose: Enter or step a bounded number without dragging.

States: Default, Focus, Disabled, Error. Text properties: Label, Value.

Semantics: Native number input and named decrement/increment buttons; bounds and errors.

Keyboard: Native editing; ArrowUp/Down step; buttons Enter/Space.

Motion: contracts/motion/interface-microinteractions.json

## Forms/DatePicker

ID: da.forms.date-picker

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=58-673)

Purpose: Choose a date or range, retaining manual entry.

States: Default, DateSelected, RangeSelected. Text properties: Month label.

Semantics: Tested date picker primitive; named dialog/grid, localized dates and week start.

Keyboard: Arrow dates; Home/End, PageUp/Down per primitive; Enter selects; Escape returns focus.

Motion: contracts/motion/interface-microinteractions.json

## Shared anatomy, tokens and layout

Semantic surface, text, action and border variables; shared Archivo type styles; space metrics and square radii. Named native layers and public text properties. Focus uses component 17:7, static triple stroke with 11px outset and 5px clear gap; never clip. Text wraps and height grows. Example widths are documentation examples, not fixed production widths. Intrinsic icons, grids and media proportions are intentional geometry.

## Implementation and evidence

Use native controls and tested headless primitives for complex patterns. Full AI A11y Toolkit reference/design.md is authoritative. Never treat drawings as keyboard or ARIA implementations. Do not improvise complex controls from these vectors. Implementation mapping: unassigned.

Before release: verify light/dark pairings and forced colors, keyboard/focus/announcements, 44px targets, 320px reflow and enlarged text, touch parity, interruption and reduced-motion alternatives, loading/error states and human review with named browser/AT pairings. Record evidence per component.

No Prime artwork, licensed components or code copied. Prime informed category breadth only. Existing live-site use is not a prerequisite for system inclusion.

<!-- Figma source: https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=58-844 · mirrored October 18, 2026 -->
