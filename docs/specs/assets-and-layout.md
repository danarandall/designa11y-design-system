# Assets, viewports and layout systems

Contract ID: da.assets-layout.v1 Owner: Dana Randall · October 18, 2026 Status: native component drafts; production behavior unimplemented/unvalidated

Original reusable assets and presentation structures. Generic payment categories and unbranded devices replace licensed template artwork. Locale names remain explicit; country flags must never stand in for language.

## Assets/BrandMedia

ID: da.assets.media

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=65-30)

Purpose: Use the correct DesignA11y identity asset for context and scale.

States: Wordmark, Symbol, Favicon. Text properties: .

Semantics: Home link named DesignA11y home; decorative duplicates hidden; never substitute favicon for clean symbol at large size.

Keyboard: Only a wrapping link is focusable.

Motion: contracts/motion/interface-microinteractions.json

## Assets/PaymentMethod

ID: da.assets.payment-method

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=65-43)

Purpose: Represent a payment category without copying licensed payment logos.

States: Card, BankTransfer, DigitalWallet. Text properties: Name.

Semantics: Visible payment method name; actual provider logos need approved official assets and license review. No current DesignA11y checkout implied.

Keyboard: Static asset; selection uses separate radio group.

Motion: contracts/motion/interface-microinteractions.json

## Assets/LocaleOption

ID: da.assets.locale

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=65-56)

Purpose: Show locale with a written language and region, independent of flags.

States: EnglishUS, EnglishUK, FrenchFR, GermanDE. Locale names and codes follow state; no shared text property can replace one locale with another.

Semantics: Use language autonyms and region text; flags represent countries, never language alone. National-flag examples are original geometry, not language labels.

Keyboard: Locale selection uses native select or tested menu; static preview is not interactive.

Motion: contracts/motion/interface-microinteractions.json

## Assets/DeviceTemplate

ID: da.assets.device

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=65-72)

Purpose: Neutral original viewport frames for interface presentations.

States: Desktop, Tablet, Mobile. Text properties: .

Semantics: Presentation-only original frame, not a device manufacturer mockup; nested screenshot requires contextual alternative.

Keyboard: Decorative presentation frame, never an interactive control.

Motion: contracts/motion/interface-microinteractions.json

## Layout/Container

ID: da.layout.container

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=65-82)

Purpose: Constrain readable content with consistent gutters.

States: Wide, Reading, Compact. Text properties: .

Semantics: Layout wrapper has no role by default; semantic section only with meaningful heading.

Keyboard: No tab stop; visual order follows DOM order.

Motion: contracts/motion/interface-microinteractions.json

## Layout/Grid

ID: da.layout.grid

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=65-110)

Purpose: Responsive content grouping with source-order consistency.

States: ThreeColumns, TwoColumns, OneColumn. Text properties: .

Semantics: CSS grid in implementation; no role from layout. Lists retain list semantics.

Keyboard: Reading and focus order follow content; no CSS order that disagrees with DOM.

Motion: contracts/motion/interface-microinteractions.json

## Layout/Divider

ID: da.layout.divider

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=65-116)

Purpose: Separate meaningful content groups without adding visual clutter.

States: Horizontal, Labelled. Text properties: Label.

Semantics: Decorative border by default; hr for thematic break; heading labels remain proper headings.

Keyboard: Not focusable.

Motion: contracts/motion/interface-microinteractions.json

## Layout/SpacingReference

ID: da.layout.spacer

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=65-129)

Purpose: Document reusable spacing scale and purposeful density.

States: Compact, Regular, Generous. Text properties: .

Semantics: Documentation reference only; use space variables instead of spacer DOM elements.

Keyboard: Not interactive.

Motion: contracts/motion/interface-microinteractions.json

## Shared anatomy, tokens and layout

Semantic surface, text, action and border variables; shared Archivo type styles; space metrics and square radii. Named native layers and public text properties. Focus uses component 17:7, static triple stroke with 11px outset and 5px clear gap; never clip. Text wraps and height grows. Example widths are documentation examples, not fixed production widths. Intrinsic icons, grids and media proportions are intentional geometry.

## Implementation and evidence

Use native controls and tested headless primitives for complex patterns. Full AI A11y Toolkit reference/design.md is authoritative. Never treat drawings as keyboard or ARIA implementations. Do not improvise complex controls from these vectors. Implementation mapping: unassigned.

Before release: verify light/dark pairings and forced colors, keyboard/focus/announcements, 44px targets, 320px reflow and enlarged text, touch parity, interruption and reduced-motion alternatives, loading/error states and human review with named browser/AT pairings. Record evidence per component.

No Prime artwork, licensed components or code copied. Prime informed category breadth only. Existing live-site use is not a prerequisite for system inclusion.
