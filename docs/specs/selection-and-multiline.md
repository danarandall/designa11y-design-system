# Forms — selection controls and multiline input

Contract ID: da.forms.selection-multiline.v1 Status: native design drafts; runtime implementation unmapped and untested Owner: Dana Randall · October 18, 2026

## Masters and API

Checkbox: node 53:122, Selection=Unchecked|Checked|Mixed × Interaction=Default|Hover|Focus|Disabled (12 variants). Radio: 53:159, Unselected|Selected × the same interactions (8). Switch: 53:200, Off|On × the same interactions (8). Each exposes Label as TEXT. Selection and interaction are independent; focus can coexist with a selected state. Disabled focus is excluded intentionally.

Textarea master is on this Forms page, named Forms/Textarea. It inherits TextField properties Label, Value, Helper text, Error message, Show helper and Interaction × Validation, with a 144px initial multiline control. Do not use entered sample values as placeholders.

## Anatomy and visual bindings

Selection: control, selection-mark, label, optional focus-indicator. Semantic surface/default, surface/subtle, text/primary, text/on-action and border/default bindings; UI/Label Archivo. Square checkbox uses radius/square; radio and switch are intrinsically round. Minimum labelled-row target is 44px. Labels wrap; containers grow. Focus uses 17:7 with 11px outset, 5px clear gap and static triple strokes. Never clip the ring. Disabled opacity is a draft treatment, not validation evidence.

Textarea: label, input-control/value, helper-text, error-message and focus-indicator. Preserve semantic colors, shared type, text growth and helper/error associations. Error is communicated through explicit text and stronger boundary, not color alone.

## Checkbox requirements

Use native input type=checkbox with an associated visible label. Space toggles. Mixed maps to the native indeterminate property and is programmatic aggregate state; user activation resolves using a documented group rule. Group related controls with fieldset/legend when appropriate. Preserve checked values after validation. Label activation operates the full target.

## Radio requirements

Use same-name native radio inputs in a labelled group. Tab enters/exits; native arrow keys move/select. Do not implement independent toggles. Required/optional group behavior and default selection must be specified by the consuming flow. Errors attach to the group and are discoverable through descriptions.

## Switch requirements

Use a tested switch primitive or button role=switch with aria-checked. Keep the accessible label stable across On/Off; state is separate. Space toggles; a button implementation also supports Enter. Use for immediately applied binary settings, such as optional effects. Avoid switch semantics for a deferred agreement checkbox. Disabled controls cannot change state.

## Textarea requirements

Use native textarea, associated visible label, contextual helper/error IDs, aria-invalid when invalid and aria-describedby as appropriate. Enter inserts a newline. Preserve native text editing and resizing. Readonly remains focusable; disabled uses native disabled behavior. Do not announce errors on every keystroke. Define validation timing in the consuming flow.

## Interface microinteractions

Microinteractions are reusable interface behavior, including new patterns not yet deployed on the site. Lab demonstrations are examples and test surfaces. Selection controls may use subtle track/fill/thumb feedback; focus itself stays static. Specify exact timing, interruption, reset, touch/keyboard parity and reduced-motion/static feedback in the linked motion recipe before implementation. Current variants are static; no native Figma animation or production code is claimed here.

## Acceptance and evidence

Design: masters exist; selection/interaction combinations, text properties and semantic bindings authored. Visual review is separate. Runtime pending: native semantics, keyboard, checked/mixed announcements, group errors, forced colors, dark mode, 320px reflow, enlarged text, target/label behavior, preference alternatives and interrupted motion. Group validation patterns, selected+error compositions and implementation mapping remain gaps.

Source: original DesignA11y assets and approved foundations. Full AI A11y Toolkit remains required. No Prime assets copied.

<!-- Figma source: https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=54-220 · mirrored October 18, 2026 -->
