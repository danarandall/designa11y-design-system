# DesignA11y contributor instructions

## Content identity and priority

DesignA11y is about inclusive design, accessibility, lived experience, and AI. It is an editorial and practical resource platform. Use authentic articles, research, toolkit resources, and inclusive-design examples.

Shared designer skills improve craft and critique. Their sample industries, travel/lifestyle imagery, narratives, and content must never override DesignA11y's identity. Dana's explicit decisions and the full AI A11y Toolkit take priority over generic creative recipes.

Figma is the primary design deliverable. GitHub supports it with versioned contracts, exports, implementation, and evidence.

## Required inputs

1. Working Figma library: https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System
2. Current site: https://www.design-a11y.com/
3. Required accessibility benchmark: https://github.com/danarandall/ai-a11y-toolkit
4. Published Figma Specs article and application: docs/figma-specs-evaluation.md

Full toolkit routing skill, design reference, and color reference were read October 18, 2026. Load the relevant full task references, not only the condensed Figma skill. Private designer-skill sources are not dependencies of this public resource.

## Approved design direction

- Elevated, editorial, restrained, and experimental. Stripe and UQ are UI references, not content or brand templates.
- Preserve existing graphics, brand artwork, and the signature corner.
- Copper remains a brand accent; the seam stays simple.
- Do not restore "INCLUSIVE DESIGN / HUMAN POSSIBILITY".
- Preserve whitespace and hierarchy. Adding copy does not substitute for a visual concept.
- Cards use neutral surfaces, restrained borders, consistent spacing, and agreed shadow-lift feedback.
- Keep Motion Lab variety inside demonstrations rather than card containers.
- Preserve mobile alignment, layer order, frame integrity, and image proportions.
- Prioritize the toolkit in homepage hierarchy.
- Do not duplicate the hero's featured article in the next article block.

Audit source values rather than inventing exact tokens from these principles. Separate observations, approved decisions, and proposals.

## Accessibility and evidence

Read skills/ai-a11y-toolkit/SKILL.md and load relevant full references before design or code work. Record revisions used. The full toolkit is authoritative; the condensed Figma version can route retrieval but is not equivalent.

Keep Figma evidence separate from runtime behavior and human/assistive-technology testing. Native Specs document intent; test agent retrieval and application before claiming performance gains.

## Typography platform mapping

Dana selected Archivo for the reusable Figma system on October 18, 2026 after reviewing tighter alternatives. Shared Body, UI and Metadata styles now use Archivo. The existing Squarespace site retains Proxima Nova intentionally; do not change the live site automatically. Anton headings and the vector wordmark remain unchanged. Inter remains documentation typography. Different font metrics require platform-specific reflow checks.

## Current action components

Figma page 34:2 contains Actions/Button (34:19; Default, Hover, Pressed, Focus, Disabled, Loading) and Actions/Link (34:32; Default, Hover, Pressed, Focus). Review instances: 34:33. Labels are native text properties. Focus uses the approved triple-stroke Focus/Indicator (17:7), 11px outset and 5px clear gap. These are review drafts with token bindings, not runtime accessibility certification. No Prime components were copied.

## Authority and changes

Dana Randall owns creative direction. Preserve valid existing IDs and bindings. Keep Figma, exports, contracts, and implementations traceable and versioned. Do not publish the repository or Community release without Dana's instruction.

## Sensory surface generation

Before creating brand imagery, read contracts/brand/sensory-surfaces.json and the Figma Backgrounds guidance (page 1:23, guide 46:2). Every image needs a declared sensory role and a continuous surface construction. Correct materials alone are insufficient: reject isolated abstract objects and object-led still lifes. For sphere-based surfaces, use many small densely packed units forming a coherent bed or terrain, rather than a hero sphere or a few floating balls.

Smooth, rough, spiky and mixed textures are all valid. Sensory support does not mean every surface must be soft or smooth. Choose texture intentionally, record feature scale and density, protect reading zones, and review intensity at final output size. Sensory preferences vary; do not claim universal comfort or therapeutic effects. Use the contract's required brief, prompt guidance, exclusions and review record. The negative image reference is composition evidence only; do not inherit its old copy or layout.

Glossy, matte, velvet, sanded and other intentional surface finishes are permitted. Treat texture and finish as separate brief fields. Encourage variety from asset to asset; preserve brand coherence through purpose, palette and continuous surface composition rather than repeating one material treatment.

## Comprehensive library retrieval and contribution

Start at contracts/library/coverage-manifest.json and docs/specs/README.md. Figma entry catalog is node 74:2. The manifest maps Prime 6 reference categories to original DesignA11y drafts and records exact master/Spec IDs, variant counts, public properties, reviewed samples and pending release work. Prime scope is a category benchmark, not a license to copy its artwork, layouts or code.

Reuse the existing compatible system component; do not rebuild one-off equivalents. For complex runtime widgets use native elements or tested behavior primitives. Figma drawings and native motion timelines do not implement DOM semantics, keyboard, ARIA or preference detection. Do not claim accessibility certification from appearance or component counts.

Microinteractions are reusable production-interface behavior, including patterns not deployed on the live site. Motion Lab demonstrates and tests them. Keeping demo/card wrappers consistent does not restrict using interaction recipes in the real interface. Read contracts/motion/interface-microinteractions.json, the linked native Spec and component guidance. Semantic state updates immediately; focus stays static; static alternatives and interruption rules are explicit.

Specs under docs/specs are versioned mirrors of native Figma Specs, not an automatic two-way sync. When changing a contract, update the native Spec, relevant master descriptions, Git mirror and manifest in the same work session; report any unresolved drift. Preserve stable IDs and public property compatibility. New components remain drafts until their release gates have evidence.

## Core-site alignment authority

Use docs/specs/resources-site-patterns.md and contracts/library/resources-site-patterns.json for the source-aligned Resources patterns. Core live-site decisions take priority over generic library drafts. Motion Lab is excluded as a layout/component reference until Dana separately approves its correction; approved motion recipes and its Resources link remain valid. The Resources parity audit records an earlier inspection; the subsequent system self-build report records published changes. Provider previews remain rights-sensitive placeholders, and page-level runtime parity is not established.


## Adapting the system to another brand

Read docs/adapt-your-brand.md and contracts/theming/requirements.json first. DesignA11y-specific creative choices describe the reference theme; a downstream project may replace its identity through a theme profile. Retain semantics, component API compatibility, keyboard/focus requirements, motion alternatives and evidence boundaries. Update theme sources and shared styles rather than overriding each component. Never claim full inheritance until the alternate-theme and binding coverage checks pass. Public Git Specs are usable without access to the working Figma file. Linked working-file IDs are provenance, not an access guarantee.
