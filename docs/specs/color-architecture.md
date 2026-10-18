# Color architecture / Variables and paint styles

System version: **0.1.0-alpha.1**.

## One palette source

The 55 brand palette steps are **color variables** in Brand · Primitives: Aubergine, Blush, Rose, Copper and Petal, each with 50–950 steps. A step does not need a duplicate paint style to work as a color source. DesignA11y is the default palette mode; Validation is an isolated test palette, not an approved replacement identity.

Brand · Semantic contains 21 purpose-based variables with Light and Dark values. UI components consume roles such as surface/canvas, text/primary, action/primary, text/on-action and border/default. Select the role by meaning; do not replace semantic bindings with a visually similar raw color.

## Paint styles

Core-color paint styles are convenience wrappers bound to their matching palette variables. The Brand/Focus pearl paint style is a composite gradient whose five stops bind to palette variables. Editing a palette source carries through its aliases and bound styles. Gradient structure, direction and stop placement are shared paint-style properties; do not claim every composite field has a native variable binding.

We intentionally do not maintain 55 duplicate paint styles. Add a composite paint style when it encodes a reusable treatment or a consuming workflow requires it. Bind its colors to variables so it does not become a second palette source.

## Brand versus functional meaning

Brand colors express identity. Functional roles such as error, warning, selection, text and focus need explicit meaning, non-color cues and validated state/theme pairings. An attractive brand accent is not automatically a safe error or warning color.

The reference anchors are Aubergine #442A42, Blush #F4DDE7, Rose #D99AAE, Copper #E8B08F and Petal #FAF7F8. Preserve their approved names; do not introduce Porcelain or Peach aliases as new official identity names.

## Adaptation acceptance

Change the palette centrally, inspect aliases, shared paints and actual component instances, then check contrast and non-color meaning for the resulting states and backgrounds. New colors invalidate old contrast evidence. Raster imagery needs its own replacement/art direction; palette variables do not regenerate it.
