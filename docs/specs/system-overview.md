# DesignA11y system contract

Owner: Dana Randall   Version: 0.1 working — October 18, 2026   Status: foundation contract; implementation and agent-performance validation pending.

## Agent entry procedure

1. Inspect this file's local collections, variables, text styles, component properties, and descriptions.
2. Retrieve the [full AI A11y Toolkit routing skill](https://github.com/danarandall/ai-a11y-toolkit/blob/main/skills/ai-a11y-toolkit/SKILL.md) and the references appropriate to the task. The condensed Figma skill is not an equivalent substitute.
3. Read the relevant token, component, and flow requirements. Name the exact source and version used.
4. Prefer an existing compatible component instance. Do not detach it to bypass its API.
5. Summarize applicable requirements and unresolved choices before building.
6. Validate measured geometry and contrast in Figma, then separately validate runtime semantics, keyboard behavior, focus, announcements, reflow, and user preferences.
7. Report evidence and remaining human review. Agent self-report is not proof.

## Four connected sources

- Toolkit: shared accessibility requirements.
- Design-system Specs: product-specific intent and behavior.
- Implemented components: actual reuse targets.
- Validation evidence: what passed, failed, and remains untested.

This structure follows [Figma Specs: Put Accessibility Into the Instructions Agents Build From](https://www.design-a11y.com/articles/figma-specs-accessibility-design-systems).

## File and token architecture

| **Source** | **Meaning** | **Use** |
|---|---|---|
| Brand · Primitives | 55 raw colors | Reference through semantic aliases for UI |
| Brand · Semantic | 15 roles, Light and Dark | Select by purpose, respecting documented pairings |
| Layout · Metrics | Source-based spacing and geometry | Bind padding, gaps, radii, and dimensions |
| Typography · Metrics | Responsive endpoints and type metrics | Preserve responsive formulas in implementation |
| Legacy · Brand anchor | Preserved original binding | Avoid for new UI |

Proposed --da-\* WEB names are an export contract, not a claim that production CSS already declares them. Existing values and IDs are preserved.

## Content identity and instruction priority

DesignA11y is about inclusive design, accessibility, lived experience, and AI. It is an editorial and practical resource platform, not a travel or lifestyle brand. Use authentic DesignA11y articles, research, toolkit resources, and inclusive-design examples. Shared designer skills are methods for improving craft and critique; their sample industries, imagery, narratives, and content must never override this identity. Dana's explicit decisions and the full AI A11y Toolkit take priority over generic creative recipes.

## Brand and composition

Retain the existing DesignA11y artwork, signature corner, copper accent, editorial restraint, and deliberate whitespace. Use neutral card containers with restrained borders; visual variety belongs in the content. Do not restore the removed “INCLUSIVE DESIGN / HUMAN POSSIBILITY” hero eyebrow. Do not duplicate the hero's featured article in the following article block.

## Typography platform mapping

Anton remains headings. Archivo is approved for reusable system Body/UI/Metadata styles; Inter remains documentation typography. The live Squarespace site intentionally retains Proxima Nova. Preserve the vector wordmark. Validate reflow for each platform.

## Accessibility decisions

- Body text: 4.5:1 minimum; large text: 3:1. Record the actual foreground/background and alpha-composited result.
- Meaningful UI boundaries and focus indication: 3:1 against adjacent colors.
- 44 × 44 CSS px preferred targets; document any use of the WCAG 24 × 24 floor and its applicable exception.
- Do not communicate information by color alone.
- Text containers grow; preserve content at 320 CSS px and enlarged text. Test spacing overrides in implementation.
- Provide keyboard access, visible unobscured focus, accessible names, and explicit focus-return behavior.
- Honor reduced motion. Do not rely on the preference alone to make motion tolerable; define calm default behavior and controls for persistent motion.
- Annotate image purpose and alternatives; a decorative image inside a clearly named article link should not repeat the title.
- Use tested behavior primitives for complex interactions rather than inventing them from drawings.

## Component contract fields

Stable name and status; purpose; source; allowed properties and combinations; structure; visual tokens; responsive rules; accessible name/role/state; keyboard model; focus; feedback; motion; image semantics; acceptance criteria; implementation mapping; evidence and limitations.

## Publication and change control

Figma is the primary design deliverable. The [companion repository](https://github.com/danarandall/designa11y-design-system) versions contracts, exports, implementation, and evidence. Native Specs retrieval works only when access is available; verify what transfers with a Community duplicate. Publish only on Dana's instruction.

## Approved system decisions — October 18, 2026

This section supersedes the earlier typography dependency paragraph: Archivo is approved for reusable Body/UI/Metadata styles; Anton remains headings, Inter documentation, and the original wordmark stays vector. The live Squarespace site intentionally retains Proxima Nova.

Focus/Indicator 17:7 uses three square 2px strokes (Aubergine / pearlescent / Aubergine), 11px outset and 5px clear gap. Keep focus static, unobscured and provide a system-color fallback in forced colors.

Brand identity includes clean Brand/Symbol 40:15, distinct from favicon, and Brand/Frame 44:55. Backgrounds guide 46:2 and contracts/brand/sensory-surfaces.json define continuous tactile surfaces. Smooth, rough, spiky and mixed textures; glossy, matte, velvet, sanded and other finishes are permitted. Encourage variety across assets.

Motion page 43:2 documents seam and Surface Field authored studies. Motion Lab remains a planned motion demonstration family, but Dana explicitly excluded the live Motion Lab layout and its inconsistent components from core-site alignment. Do not use that page as a layout/component authority until it is separately corrected. Approved microinteraction contracts remain reusable in production interfaces. Preserve neutral wrappers and place variety inside demonstrations.

Runtime semantics, keyboard, assistive technology, reflow, motion tolerability and agent retrieval remain validation work. This library is not yet comprehensive or release-ready.

<!-- Figma source: https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=12-2 · mirrored October 18, 2026 -->
