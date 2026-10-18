# Figma Specs evaluation

Status: published article read October 18, 2026; native Specs integration remains proposed and untested.

## Authoritative article

[Figma Specs: Put Accessibility Into the Instructions Agents Build From](https://www.design-a11y.com/articles/figma-specs-accessibility-design-systems), Dana Randall, October 17, 2026.

## Architecture to apply

Use four connected sources with clear responsibilities:
1. AI A11y Toolkit: shared accessibility requirements.
2. Design-system Specs: product-specific token, component, content, behavior, and flow decisions.
3. Implemented component library: actual reusable components.
4. Validation evidence: tested behavior, failures, and unresolved human-review work.

Maintain agreement between written intent, Figma representation, and implemented behavior. Avoid competing copies.

## Requirements derived from the article

- Establish platform, implementation constraints, ownership, and versioned accessibility foundations before component generation.
- Explain intended token use, approved foreground/background pairs and contrast calculations, interaction states, text growth, reflow, target sizes, and user preferences.
- Component contracts specify meaning and accessible names, interaction alternatives, focus entry/movement/return, feedback, and adaptation.
- Flow guidance covers reading order, validation, recovery, progress, preserved input, submission outcomes, and descriptive content.
- Write observable acceptance criteria, including dynamic preference changes where relevant.
- Agent workflow must retrieve foundations and relevant token/component/flow guidance, identify the implementation to reuse, summarize requirements and gaps, then implement and report validation.
- Confirm intended content loaded before interpreting scans. Include manual keyboard, assistive technology, reflow, resizing, alternative-text, and content review.
- Feed failures into both implementation and guidance.

## Proposed native Specs use

Evaluate native Figma Specs for these explanations close to design assets. Keep structured tokens, schemas, implementation, and tests versioned in GitHub. Link to exact component IDs, contract versions, and repository revisions.

## Evaluation before adoption

- Verify Specs availability for the plan owning the target file; never infer ownership from another plan.
- Test whether the intended agent discovers, retrieves, and applies the relevant guidance.
- Compare the condensed skill against the same skill plus fuller Spec guidance with identical tasks and scoring.
- Record source versions, agent environment, outcomes, failures, and manual-review requirements.
- Check what transfers when a Community file is duplicated and what requires external access.

The article presents improved agent performance through Specs as a hypothesis to test. Do not describe documentation presence, agent self-report, or a clean scan as proof of accessibility.
