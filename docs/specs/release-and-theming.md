# Release, theme inheritance and evidence

System version: **0.1.0-alpha.1**. Status: **prerelease; Figma Community unpublished**. The public GitHub documentation is available; that does not imply a published or validated Community library.

## Version model

A release version identifies a coordinated snapshot of Figma masters, variables, styles, native Specs, Git mirrors, contracts and available implementation mappings. A schemaVersion such as da.brand.identity.v1 identifies a data shape, not the system release. Component IDs remain stable across compatible updates.

Before 1.0, breaking APIs still require explicit migration notes and a minor-version increment. Alpha revisions record ongoing work. After 1.0: major for breaking token/property/behavior APIs, minor for compatible features and patch for compatible fixes. Freeze a release record with exact Git commit and Figma version or duplicate URL; never silently edit an immutable release record. Working main/file may continue evolving. Do not assign 1.0 until the stated release gates have evidence.

## Learnings incorporated

- Shared text-style font families, styles, sizes, line heights and tracking now bind to central variables. Local component typography was connected to central font roles.
- Brand pearl gradient stops bind to the palette; shared shadow/effect values bind to variables.
- Component control/surface radius roles are separate from intentionally square/fixed geometry.
- Paired promos, equal-height resource cards, growing content and responsive stacking are reusable composition requirements.
- Validate components inside consuming layouts and CSS/style systems; inherited foreground/background rules can break a correct isolated component.
- Specs and contracts need exact production mappings and evidence references; missing implementations must be explicit, never fabricated.

## Theme validation evidence

Review board: 118:3 on page 118:2. Same genuine button (34:3), field (38:3) and card (87:174) masters are instantiated in two isolated theme contexts. Source masters and DesignA11y defaults are unchanged.

Reference: Anton/Archivo, Aubergine/Petal and square component corners. Validation: Inter, teal/cream and 8px control/surface corners. Shared gradient/effect styles inherit mode choices. Sample text/action contrast: reference 11.91:1, validation 8.58:1. Visual review found the sampled content visible and reflowing. Field wrapper remains unpainted/square; its input surface carries the control radius.

This establishes inheritance for sampled instances, not every family/state/theme. Dark mode, non-text contrast, extreme text, localization, preference settings and runtime behavior still require their own evidence. Validation is not a newly approved brand identity.

## Current product scope and audit

The current goal is brand-adaptable Figma driven by the DesignA11y adaptation agent. A separate headless code-component library is not the current deliverable. Runtime requirements stay documented for downstream implementers and must not be described as implemented by Figma.

Typography binding audit: 984 eligible own-master text nodes across 87 component sets on 11 pages; zero missing eligible font-family bindings in that audit. Seven hover-container radius omissions were identified and repaired. Brand geometry and untouched asset shapes are intentional exceptions. This is structural evidence, not a claim that every state was visually or accessibly validated.

Native Check designs was searched in this Pro file and unavailable. Figma documents it for Organization/Enterprise: https://help.figma.com/hc/en-us/articles/39592284074263-Check-designs-in-Figma . Record not run, not passed. Use it in supported consuming files alongside direct binding and visual review; inspect semantic intent before applying suggestions.

## Platform-neutral release gates

| **Gate** | **Required evidence** |
|---|---|
| Identity | All eight brand categories defined or explicitly not applicable; mission, POV and audience retained |
| Bindings | Themeable masters use variables/shared styles; literals and fixed geometry have justified exceptions |
| Theme propagation | Palette, typography, radius, gradient and effects tested on real instances; report family/state coverage |
| Content and composition | Long/short/localized content, wrapping, equal-height rules, narrow and wide layouts without clipping |
| Semantics and interaction | Native elements or tested primitives; names, roles, states, keyboard, focus, errors and announcements |
| Visual accessibility | Actual state/theme text and non-text contrast, focus visibility, forced colors, zoom/reflow/spacing |
| Motion and media | Meaningful purpose, immediate semantics, static alternatives, interruption and user preferences |
| Traceability | Component ID/API → Spec → token/style/asset map → implementation or explicit unmapped status → evidence |
| Validation truthfulness | Live runtime, exported representation, source inspection and human/AT results distinguished; blocked is not passed |
| Rights and privacy | Original/rights-cleared distributable assets, usable public links, no private references/history |
| Copy and retrieval | Duplicate preserves variables/styles/components/Specs; independent agent can retrieve exact requirements |
| Version parity | Cover, VERSION, release manifest, Specs and changelog agree; migration notes and known limitations included |

## Implementation mapping contract

Each family records systemVersion, stable componentId, Figma file/master/property API, native Spec ID, public Spec path, token/style dependencies, platform-neutral behavior, implementations (repository/path/export/revision/support status), tests/evidence (environment/date/method/result) and known limitations. Use null plus a reason for absent code. Never mark a Figma design as a runtime implementation.

## Publication decision

This alpha remains a working reference. Community release waits for the declared gates and Dana's publication instruction. Keep unresolved gates visible; never convert a pending check into a pass because documentation exists.
