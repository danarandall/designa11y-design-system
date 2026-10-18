---
name: designa11y-adapt-brand
description: Guide a brand interview and adapt a duplicated DesignA11y Figma design system through central variables, styles and asset slots while preserving accessibility requirements. Use when users ask to rebrand, customize or theme a copy of DesignA11y, define its brand profile, or validate inherited styling.
---

# DesignA11y brand adaptation

Treat this as an experimental skill for system version 0.1.0-alpha.1. Do not claim successful end-to-end validation until evidence exists for the user's copied file. A skill supplies instructions; it does not grant tool access.

Read [workflow.md](references/workflow.md), [identity.md](references/identity.md), and [release-gates.md](references/release-gates.md) before applying changes. Consult [color.md](references/color.md) for palette architecture.

## Establish the target

Ask for the user's duplicated Figma file and intended channels. Inspect the destination file and its release metadata through available Figma tools. Never use the DesignA11y source file as the adaptation destination. If the user supplies the source, guide duplication first. If duplication is unavailable through tools, request the copied file URL; continue the interview meanwhile.

Use installed Figma skills and supported APIs; inspect actual IDs and bindings in the copy. Source-file node and variable IDs are references, not portable identifiers. Resolve by collection, role, style and component names, detect duplicates, and record a destination mapping. Verify font availability and applicable access before writes. If write access is absent, deliver a profile and application plan without claiming Figma was changed.

## Interview

Reuse answers already supplied. Ask two or three related questions at a time and offer concrete choices without inventing approved decisions. Cover:
- Brand mission, audiences, context, emotional intent, distinctive point of view and prohibited associations.
- Primary/secondary marks, wordmark, symbol, monochrome and small-format variants; supplied assets and usage rights.
- Signature colors and emotional roles, separate from functional UI semantic roles.
- Heading/display/body type, weights, readability, language coverage, available fonts and licensing.
- Graphic motifs, patterns, frame/divider language and composition.
- Custom icon/illustration direction, stroke, shape, detail, alongside functional icon legibility.
- Photography, image references, subjects/casting, lighting, grading, crop, texture and background function.
- Voice, vocabulary, channel tone, example copy and prohibited claims.
- Motion personality, pacing and purpose; reduced-motion and static alternatives.
- Radius, spacing/density, borders, shadows, gradients, hierarchy and responsive behavior.
- Web UI, social, video, packaging or other intended applications.

Treat DesignA11y's inclusive-design-and-AI context and tactile Surface Field as the source brand's reference identity. Do not force that mission, name, motifs or sensory art direction onto another brand. Retain accessibility rules and functional contracts.

## Record and review

Produce a machine-readable brand profile with schemaVersion, sourceSystemVersion, destinationFile, brandContext, identity, theme, assets, channels, accessibilityRequirements and decisions. For each decision record value, status (approved/proposed/pending/not-applicable), rationale and affected roles. Make unknowns explicit. Separate aesthetic decisions from accessibility requirements.

Show a concise proposed change list and unresolved choices. Obtain approval for the concrete brand profile before applying identity changes, unless the user has already approved those exact choices. Do not repeatedly request approval for authorized application steps.

## Apply

Create a recoverable checkpoint or describe the available undo/version mechanism. Apply approved central palette variables and semantic aliases, typography variables/styles, shape and effect sources, and composite gradient styles. Preserve semantic names, component properties, variants, states, auto-layout and nested instances. Replace marks and imagery through shared asset masters where possible. Do not regenerate a wordmark by changing its font, detach instances to recolor them, or scatter raw values across component instances.

Record controlled exceptions such as logo geometry, fixed focus geometry and channel canvas dimensions. Image assets require their own art direction and replacement; palette changes do not recolor or regenerate them.

## Validate and deliver

Compare baseline and adapted instances from Actions, Forms, Navigation, Content, Feedback, Overlays and Data. Exercise relevant themes, interaction states, long copy, responsive widths, truncation, overflow and available fonts. Inspect alias resolution and unexpected overrides; report actual coverage and missing bindings.

Recheck contrast for changed foreground/background and state pairings, non-color cues, visible focus, target sizes and reduced-motion alternatives. Use native Figma checks when available; mark unavailable checks as not run. Figma checks do not establish runtime keyboard, semantics or assistive-technology conformance. Use the user's accessibility toolkit for implementation validation when a runnable implementation exists.

Deliver the profile, destination links, change log, measured evidence, exceptions and remaining creative/manual tasks. Keep source/version attribution transparent. Do not publish a Community file, deploy a site, install a plugin or claim certification as a side effect of adapting a file.
