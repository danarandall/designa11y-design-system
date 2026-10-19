# DesignA11y adaptation agent / Figma-first workflow

System version: **0.1.0-beta.1 · Public beta**. The [experimental adaptation skill](../../skills/designa11y-adapt-brand) and [standalone starter prompt](../adaptation-prompt.md) are available. This contract describes the guided workflow; it does not claim an autonomous hosted service or complete alternate-brand inheritance.

Guide a brand owner through context, identity and cross-channel expression, then apply approved choices centrally to a copy of the Figma system while retaining accessibility requirements.

## Unified inputs

The website-derived foundations and functional component contracts remain the system baseline. The brand identity contract adds eight identity domains. The expression contract adds original motifs and channel rules. The resulting profile defines a new brand's own POV; DesignA11y is the reference theme, not mandatory styling.

Identity Spec: 119:134. Cross-channel expression Spec: 123:1319. Release and evidence Spec: 119:246.

## Guided interview and application

1. Retrieve the versioned public contracts and current native Specs; verify the Figma source and target permissions.
2. Ask a short context interview: mission, audience, POV, content, channels and constraints.
3. Prefill documented existing brand decisions with source and status; ask what should change rather than restarting an established identity.
4. Ask about all eight identity categories and applicable cross-channel expressions; allow not applicable with a reason.
5. Create a brand profile with field-level approved/proposed/pending/not-applicable status, examples, exclusions, source and rationale.
6. Review the proposed identity/theme mapping and surface accessibility or rights conflicts before applying it.
7. Create a separate Figma copy and record source/copy versions; preserve original reference masters.
8. Apply approved colors, font roles/metrics, radii, gradients/effects, asset-master replacements and supported layout/motion values centrally.
9. Preserve instances, component properties, aliases, accessibility contracts and content context; do not detach components or add ad hoc per-instance aesthetics.
10. Apply brand-specific imagery and motifs through shared masters; treat image/logo creation as separate creative work requiring explicit direction and review.
11. Run native Check designs where available; record tool availability, scope, suggestions and reviewed exceptions. Never bulk-apply approximate matches without reviewing meaning.
12. Audit bindings and actual resolved values; test representative states, content extremes, aspect ratios, preferences and dark/light choices; review visually.
13. Deliver the Figma copy, approved brand profile, token/style/asset mapping, updated copy-specific Specs, version/changelog and truthful evidence/known gaps.
14. Do not publish the customized copy or Community release automatically.

## Profile requirements

Mission, audiences, point of view, content context and channels come first. Every identity category records decisions, source, owner, rationale, examples, exclusions and approved/proposed/pending/not-applicable status. Applicable channels add pattern/background grammar, composition and production/accessibility requirements. Do not silently promote an inferred suggestion to an approved decision.

Apply central variable/style/asset changes to a copy and preserve component connections. Changing a font does not redraw a wordmark; changing palette tokens does not recolor an embedded raster photograph. Record manual creative tasks. The agent must not force sensory surfaces or copied reference artwork into an unrelated identity.

## Reference-theme campaign imagery

For DesignA11y social and campaign images, use the brand symbol as a window or image mask, with deliberate negative space. Retire the repeated “frame echo” pattern as a campaign expression.

Two approved creative directions are:

- **Human window:** a person looks through or holds the symbol like a window. The image lives inside the window, with a selective part of the subject extending beyond the open corner.
- **Window with spill:** imagery lives inside the symbol, while a restrained group of particles or image-related elements sprinkles out through its open corner.

Preserve the actual symbol geometry and its open corner. Keep the window legible, the spill intentional and the surrounding composition spacious. These are campaign treatments, not default interface decoration or replacements for the wordmark. Figma campaign samples are creative references requiring refinement and review, not evidence of finished production artwork.

During adaptation, replace this reference-theme expression with the new brand's approved symbol and image grammar, or mark it not applicable. Do not carry DesignA11y artwork into another identity or force an unsuitable logo into a window. Record imagery, masking and compositing work separately from token changes. Provide appropriate text alternatives for meaningful imagery; keep essential copy outside image-only treatments and revalidate contrast at each intended crop.

## Accessibility and reporting

Retain requirements and revalidate the resulting design. Figma evidence does not establish runtime semantics, assistive-technology usability or universal accessibility.

Public machine entry: https://github.com/danarandall/designa11y-design-system/blob/main/contracts/agents/brand-adaptation-agent.json
