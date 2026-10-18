# Adaptation execution / Learnings from incomplete tests

Status: working prerelease refinement. An incomplete test can reveal defects; it does not establish a complete adaptation or accessibility pass.

## Preserve configurable content
Central STRING variables provide defaults through the owning component or component set's TEXT property defaultValue. Text layers keep their characters component-property reference. Instance property values remain available for distinct titles, descriptions and captions.

Do not directly bind characters on a layer controlled by a TEXT property: the binding can clear that reference and hide instance overrides. Snapshot and compare property names, types, variant counts and representative instance values. Verify that differently configured instances still show different copy.

In the master, 143 additional text-layer connections across editorial, responsive and resource components were restored. The 20 affected component sets retained property names and variant counts. This count excludes the earlier promo-panel repair.

## Content determines height
Footer columns must hug content rather than retain a 48px construction height. Source footer variants now grow around the brand statement and link groups. Check narrow layouts, longer localized copy, replacement fonts and actual descendant bounds. A container having clipsContent=false does not make overflow acceptable.

## Research has a defined purpose
Start with the user's approved brand profile, supplied assets, embedded Specs and system contracts. Research a specific missing fact only when needed; use authoritative sources when verification is required. End the search when the fact is sufficiently answered. Record missing permissions or assets and proceed with independent approved work. Do not expand a rebrand into open-ended asset discovery or repeat successful URL checks without a new reason.

## Render each typography role
Host font availability, rendered appearance and licensing are separate questions. Test actual layers for each role, including requested monospace text and weights. Do not infer a rendering pass from a font menu entry. Preserve available-font evidence without representing it as permission to distribute a font.

## Work in verifiable batches
Apply central theme, component defaults, example-copy overrides, assets, motion and layout/state checks in coherent batches. Read back each batch before marking it complete. Keep a checkpoint containing source revision, destination, approved profile, current stage, changed IDs, asset dispositions, completed checks, blockers and next action. Parse structured checkpoints on readback. Resume from evidence rather than repeating the interview or earlier research.

## Honest completion
Report what was changed, what was checked and what remains. Distinguish user-reported observations from independently verified evidence. A palette/typography pass is useful partial progress; it does not mean artwork, motion, responsive behavior, keyboard interaction or assistive-technology checks passed.

## Next regression
Use a fresh copy and the same approved test profile. Verify distinct component overrides, growing footers, source-brand asset dispositions, role-specific radii, actual font rendering, long labels, responsive layouts and clear Spec placement. Do not publish automatically.
