# Adapt without installing a skill

You can use the prompt below with an AI assistant that can read the system's guidance. A compatible Figma connection with write access is needed to apply changes; without it, the assistant can prepare the brand profile and instructions. The prompt does not install a skill or grant access. Results still require validation.

Duplicate the file first. Replace the bracketed fields, copy the entire prompt into your assistant, and keep the approved brand profile with your copy.

## Copy this prompt

```text
Help me adapt a copy of the DesignA11y design system to my brand.

My copied Figma file: [PASTE COPIED FILE URL]
My brand name and website, if available: [ADD HERE]
My intended uses: [WEB / SOCIAL / VIDEO / PACKAGING / OTHER]

First verify that the destination is my copy, inspect its version and structure, and explain what your current tools can read and edit. Do not edit the original DesignA11y file. If you cannot access Figma, complete the interview and deliver a structured brand profile and an application plan; do not claim the file was changed.

Read the system's embedded Specs and public guidance:
https://github.com/danarandall/designa11y-design-system/blob/main/docs/specs/brand-identity.md
https://github.com/danarandall/designa11y-design-system/blob/main/docs/specs/adaptation-regression.md
https://github.com/danarandall/designa11y-design-system/blob/main/contracts/theming/adaptation-map.json
If any source is unavailable, identify the gap instead of inventing its requirements.

Ask me a few related questions at a time. Reuse information I already gave you. Cover:
1. Mission, audiences, context, emotional intent and point of view.
2. Logos, wordmark, symbol, small-format and monochrome variants.
3. Signature colors and their brand roles, separate from functional UI colors.
4. Display and body typography, weights, language coverage and available fonts.
5. Graphic motifs, patterns, illustration and icon style.
6. Photography, backgrounds, textures, composition and image references.
7. Voice, tone, vocabulary and example content.
8. Motion personality, purpose, pacing and static/reduced-motion alternatives.
9. Control and surface corner radii, spacing, borders, shadows and gradients.
10. Channel requirements and the supplied assets we may use.

Produce a machine-readable brand profile. Mark choices approved, proposed, pending or not applicable. Present the proposed changes for my review before applying them, unless I already approved those choices.

Apply approved choices through central variables, aliases, shared styles, Brand · Content string variables and shared image/mark masters. Discover names and IDs in my copy; source IDs may differ. Preserve component structure, variants, properties, accessibility requirements and functional meaning. New colors require new contrast checks. Palette changes do not regenerate raster artwork.

Inventory every page and give each source-brand asset or content group a disposition: replace, retain-approved, omit or pending. Include backgrounds and their prompt guidance, logos and patterns, motion/social/video artwork, editorial placeholder images, author/content samples, responsive templates, resource patterns, routes and captions. Do not leave DesignA11y's mission or sensory art direction in my brand by default. Preserve truthful source attribution separately.

Check inherited changes across component families, interaction states and responsive widths. Inspect all four corner binding fields; preserve approved fixed geometry such as focus indicators and page canvases. Test long palette names and replacement copy for clipping and awkward wrapping. Keep Specs clear of design frames. Check local overrides, raster fills, vector artwork and motion timelines as well as visible text.

Finish with links to changed designs, a change log, test evidence and every unresolved item. Distinguish Figma checks from runtime keyboard and assistive-technology testing. Do not call the adaptation complete while unresolved source-brand content remains. Do not publish the file or deploy a website automatically.
```

## Optional skill

The [DesignA11y adaptation skill](https://github.com/danarandall/designa11y-design-system/tree/main/skills/designa11y-adapt-brand) packages the workflow for compatible assistants. It is optional. Both entry points require the same review and validation; neither guarantees complete adaptation.
