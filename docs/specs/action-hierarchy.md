# Actions — hierarchy and size expansion

Contract ID: da.actions.expanded.v1 Status: native design drafts; runtime validation pending

Secondary, Tertiary and Destructive button sets extend the existing primary Button. Each exposes regular/compact × Default, Hover, Pressed, Focus, Disabled, Loading. Compact minimum target is 44px; regular 48px. Original primary IDs remain compatible.

Keep existing Label and Loading label public properties. Use native button with explicit type. Enter/Space activate once; loading announces pending state, prevents duplicate submission and preserves focus. Disabled uses native disabled only when appropriate. Destructive actions require explicit labels and recovery/confirmation matched to consequences; no invented error hue or color-only meaning.

Focus remains the approved static triple stroke. Reduced motion uses static feedback. Apply da.motion.action-feedback only after component/runtime review. Text wraps and buttons grow; avoid fixed widths in implementation.

Remaining evidence: theme contrast, forced colors, content extremes, keyboard/AT, interrupted loading, responsive groups and production mappings. No Prime assets copied.

## Actions/ButtonSecondary

Master: 62:53 · 12 variants

## Actions/ButtonTertiary

Master: 62:86 · 12 variants

## Actions/ButtonDestructive

Master: 62:119 · 12 variants

<!-- Figma source: https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=62-152 · mirrored October 18, 2026 -->
