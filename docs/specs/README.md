# DesignA11y Specs index

Figma is the primary design deliverable. These Markdown files mirror native Figma Specs and are versioned with the machine contracts. Synchronization is explicit, not automatic.

[Open the Figma library catalog](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=74-2)

## Read order

1. [System overview](system-overview.md) and [coverage](library-coverage.md).
2. The relevant family Spec below and native master description.
3. [Coverage manifest](../../contracts/library/coverage-manifest.json), relevant brand/motion/component contracts, and the full [AI A11y Toolkit](https://github.com/danarandall/ai-a11y-toolkit).
4. Validation evidence and known limitations before implementation or publication.

## Native Spec mirrors

| Spec | Native Figma source |
|---|---|
| [extended forms](extended-forms.md) | [Open Spec](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=58-844) |
| [navigation](navigation.md) | [Open Spec](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=59-278) |
| [feedback and status](feedback-and-status.md) | [Open Spec](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=60-231) |
| [content and editorial](content-and-editorial.md) | [Open Spec](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=61-272) |
| [overlays and groups](overlays-and-groups.md) | [Open Spec](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=63-176) |
| [data and lists](data-and-lists.md) | [Open Spec](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=64-245) |
| [assets and layout](assets-and-layout.md) | [Open Spec](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=65-205) |
| [responsive patterns](responsive-patterns.md) | [Open Spec](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=68-456) |
| [action hierarchy](action-hierarchy.md) | [Open Spec](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=62-152) |
| [interface microinteractions](interface-microinteractions.md) | [Open Spec](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=55-89) |
| [system overview](system-overview.md) | [Open Spec](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=12-2) |
| [library coverage](library-coverage.md) | [Open Spec](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=52-8) |
| [selection and multiline](selection-and-multiline.md) | [Open Spec](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=54-220) |
| [icons](icons.md) | [Open Spec](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=66-211) |
| [typography scale](typography-scale.md) | [Open Spec](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=70-18) |
| [effects and motion metrics](effects-and-motion-metrics.md) | [Open Spec](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=71-22) |

## Current evidence

This expansion adds 67 component families and 232 variants. Nine component/pattern pages contain 75 component sets and 295 variants including earlier work. The build also adds 24 original interface icons, four illustrative country flags, seven type styles, three effect styles, four motion metric tokens and four native motion studies. Representative visual compositions and top-level bounds were reviewed; this is not every variant in every theme.

Every Prime reference category has a mapped original draft or an explicit original alternative. This is representative category breadth, not an identical licensed asset pack or a production-ready parity claim. Payment/provider artwork uses generic categories and slots; device frames are unbranded; flag/icon packs are not exhaustive. Pricing and review content is illustrative.

## Updating a component

- Preserve stable IDs and property compatibility; reuse compatible instances.
- Name purpose, anatomy, properties/defaults, valid states, tokens, responsive rules, semantics, keyboard/focus and motion.
- Use native elements or tested primitives for production interactions. Record the actual implementation mapping and version; currently unassigned.
- Update the native Spec, Git mirror, component description and coverage manifest together. Note unresolved drift.
- Keep design evidence, native timeline authoring, runtime checks and human/AT evidence separate.
- Before release, verify themes/contrast, forced colors, 320px and text growth, keyboard/AT, touch, preferences, interruption and content extremes.

## Motion

Microinteractions belong to the real interface, including patterns not yet on the live site. Motion Lab is a demonstration and evaluation surface. The [interface contract](../../contracts/motion/interface-microinteractions.json) contains proposed recipes and approved card lift. Static alternatives, immediate semantic state and interruption handling are required. Native studies at node 67:89 do not implement production triggers or preference detection.

## Redistribution

No Prime components, icons, source code or artwork are included. Its page-category inventory informed breadth. Publish the Figma Community reference only on Dana Randall's instruction after a duplicate-transfer and provenance review.

## Core-site Resources alignment

[Resources site patterns](resources-site-patterns.md) · [native Spec](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=96-1063) · [machine map](../../contracts/library/resources-site-patterns.json). Eight source-aligned component families and wide/narrow editable assemblies were added after the breadth inventory above. Keep category coverage separate from verified live-site parity. Motion Lab layout is excluded. See the Spec for publication and runtime gaps.


## System self-build and adaptation

- [System resource-page implementation Spec](system-resource-page.md), native source 108:1116.
- [Workflow validation report](../research/system-self-build-report.md), native source 109:1116.
- [Brand adaptation guidance](../adapt-your-brand.md).
- [Single-source theming requirements](../../contracts/theming/requirements.json).

All Specs in this directory are public Markdown guidance. The working Figma file may require permission; it is not a prerequisite for reading these contracts. Automatic two-way synchronization and complete theme propagation are not claimed.
