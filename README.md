# DesignA11y Design System

An evolving reference for design systems that humans and AI agents can understand, use and adapt to another brand.

## Start here

- [Adapt the system to your brand](docs/adapt-your-brand.md)
- [Public Specs index](docs/specs/README.md)
- [Machine-readable component inventory](contracts/library/coverage-manifest.json)
- [AI contributor guidance](AGENTS.md)
- [Single-source theme requirements](contracts/theming/requirements.json)
- [Workflow validation report](docs/research/system-self-build-report.md)
- [Live system page](https://www.design-a11y.com/design-system)
- [Full AI A11y Toolkit](https://github.com/danarandall/ai-a11y-toolkit)

## What is available

Public Markdown Specs and JSON contracts describe foundations, component purpose, native Figma IDs, properties, states, composition, sensory surfaces, motion and accessibility acceptance criteria. The Specs can be read and adapted directly here; access to the working Figma file is not required. The Figma Community release remains planned. Working-file links are provenance and may require access.

This is an active reference build. Representative component breadth exists in Figma, but production component mappings, comprehensive runtime validation, automatic token export/synchronization and complete alternate-brand inheritance are not yet delivered. Do not infer readiness from component counts. The inventory and individual Specs record pending checks.

## Adaptation model

Brand theme → semantic roles → shared component styles → instances and implementations.

DesignA11y is the reference identity. Replace its colors, fonts, radii, gradients, shadows and other theme values centrally. Preserve inclusive behavior and revalidate visual accessibility and reflow. The [theme requirements](contracts/theming/requirements.json) specify the required second-theme test; full propagation remains a release gate, not a current guarantee.

## Repository boundary

This repository contains distributable guidance and contracts with a clean public history. Private source folders, licensed reference links, site deployment material and the original working history are maintained separately and are not dependencies of this resource. Never merge private history or publish private source links here. See [publication boundaries](docs/publication-boundaries.md).

## License and identity

Original files distributed here are available under the [MIT License](LICENSE). Keep the copyright/license notice when adapting. External resources retain their own terms. The license does not grant trademark rights or rights to linked website imagery, proprietary fonts, Prime assets or material outside this repository. Replace DesignA11y names, logos, contact details and brand assets with your own; do not imply endorsement. See [NOTICE](NOTICE.md).

## Evidence

The self-build is an implementation case study, not a controlled proof that Specs improve agent performance. Captured-DOM scans are distinct from live-route scans, and human/assistive-technology checks remain queued. Accessibility is a property of the resulting experience and must be evaluated after adaptation.
