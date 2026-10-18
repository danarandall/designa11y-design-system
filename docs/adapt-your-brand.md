# Adapt the system to your brand

The reusable resource is the system architecture, contracts and accessibility guidance. DesignA11y's inclusive-design and AI identity is the reference implementation; your product supplies its own identity and content context.

## Change the theme once

Use a brand theme as the source for primitives. Semantic aliases describe purpose (text/primary, surface/default, border/default, action/primary, focus/outer), rather than a particular hue or font. Components consume semantic values or narrowly justified component aliases. Instances inherit the master bindings.

| Theme input | Required propagation |
| --- | --- |
| Palette and light/dark choices | Text, surfaces, strokes, states, focus and gradient stops |
| Font families and typography roles | Shared text styles, headings, body, UI labels and metadata |
| Radius scale | Component corner bindings, with documented exceptions |
| Gradients | Shared paints assembled from tokenized stops and geometry |
| Shadows/elevation | Shared effect styles and implementation tokens |
| Spacing/density, strokes and icon style | Supported semantic/component bindings |
| Motion timing/easing | Shared recipes while preserving static alternatives and immediate semantic updates |

Figma variables support only particular fields. Use shared text, paint and effect styles for composite values, with explicit token-to-style mappings and a documented update process. Do not promise that every field is natively bindable or that changing Git automatically updates Figma. Native Specs, exported tokens and runtime code require reviewed synchronization.

## Human workflow

1. Duplicate the eventual distributable library or work from these public Specs/contracts. The working Figma file is not yet a published Community package.
2. Define your identity, content context and theme values centrally. Obtain font and asset rights; no proprietary font files are included here.
3. Remap semantic roles to your theme. Preserve stable APIs; do not edit every component instance or detach it.
4. Update composite styles through the documented adapter. Record intentionally fixed geometry and unsupported fields.
5. Check a representative page and component states across responsive sizes, themes, enlarged text and long/localized content.
6. Validate text/non-text contrast, focus, forced colors, keyboard/AT behavior and motion preferences; record unresolved issues.

## Agent instruction template

> Apply the supplied brand identity through the central theme layer. Read the theming contract, component inventory and relevant Specs first. Preserve semantic role names, component properties, accessibility behavior and validation boundaries. Bind components to shared theme values; do not create isolated per-instance overrides. Report unsupported mappings and hard-coded exceptions. Demonstrate the change on representative components before claiming inheritance. Run the full relevant accessibility toolkit references and record actual evidence.

## Acceptance test

Create a clearly different test brand: new palette, font family, radius, gradient and shadow. Switch the theme boundary without editing individual masters/instances. Audit all component families for raw aesthetic values, detached styles and unresolved aliases; verify representative actions, inputs, navigation, cards and overlays. Capture before/after evidence and Figma/code resolved-value parity. A changed color alone does not establish typography, radius, gradient or effect inheritance.

Current status: the required architecture is recorded; a complete binding audit and alternate-theme propagation test are pending. No full-library single-change guarantee is made yet.
