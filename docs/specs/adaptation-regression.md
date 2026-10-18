# Adaptation regression / Nightjar findings

Status: master remediation implemented; fresh-copy regression still required. Source appearance remains DesignA11y.

## What the first test demonstrated
The first Nightjar adaptation was mostly successful according to the owner's visual review. It revealed incomplete adaptation of backgrounds, motion/social artwork, editorial imagery, responsive copy and resource patterns; longer palette labels and documentation placement also needed repair. This is qualitative evidence, not an independently measured full-file pass.

## Required adaptation inventory
Classify every item as replace, retain-approved, omit or pending. Unresolved items block a complete-adaptation claim.
- Identity marks: wordmark, clean symbol, favicon and frame.
- Backgrounds: Settle, Orient and Explore raster treatments, plus all crop variants and prompt families.
- Motion: static Surface Field, seam static and timed geometry, social square, brand video frames and all timelines.
- Content: editorial titles, descriptions, author identity, metadata, captions, tags and placeholder media.
- Responsive templates: homepage, article, toolkit landing, search, preferences and motion demonstration content.
- Resource patterns: hero, featured panels, topic links, rows, showcases, paired cards, example destinations and inverse variants.
- Documentation: source-brand art direction versus reusable functional guidance. Preserve truthful source attribution.

Do not treat a matching image hash as sufficient evidence that two asset roles are equivalent. Inspect shared image-style usage and local overrides. Inspect all four individual corner binding fields.

## Central sources
Brand · Content supplies shared STRING variables for reusable sample copy and palette display names. Stable semantic keys are independent of display labels. Do not rename semantic APIs just because a brand uses a new color name.

Brand/Assets/Surface/Settle, Orient and Explore paint styles hold raster sources. Brand/Assets/SurfaceField/Static is a separate motion poster slot. Palette variables do not regenerate these images.

Brand · Shape supplies radius/control and radius/surface. Ask for both, including an explicit zero when square is intentional. Preserve approved fixed geometry for page canvases, focus indicators, glyphs and state mechanics; do not silently inherit square corners from the source.

## Layout and evidence
Test longer palette names at 254px label width and longer sample copy at actual responsive widths. Native Specs belong outside design bounds with a 320px gutter and 240px vertical separation, recalculated after layout changes.

Audit every page's text, vector artwork, raster fill and motion content for source-brand remnants. Record each retained source-brand occurrence and its reason. A static image replacement does not establish an animated motif replacement. If motion capabilities are unavailable, record pending work rather than claim completion.

## Acceptance
Deliver a resolved brand/content/asset inventory, binding audit, screenshots of representative default/focus/error/disabled and narrow layouts, contrast evidence for changed pairings and an explicit manual/runtime test boundary. Retest a fresh duplicate after source fixes. Never publish or certify automatically.
