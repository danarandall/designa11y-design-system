# Resources site patterns

Contract ID: da.pattern.resources.v1
Status: source-aligned draft; runtime accessibility verification pending
Source: https://www.design-a11y.com/designer-resources
Inspected: 2026-10-18, rendered desktop DOM and CSS. Narrow layout derived from source rules; live mobile interaction was not exercised.

## Source authority

DesignA11y concerns inclusive design, accessibility, lived experience and AI. Preserve Dana's approved decisions and the full AI A11y toolkit above generic design recipes. Core site designs inform site patterns. Motion Lab is excluded as a layout/component reference until separately corrected. Its resource link and approved motion behavior may still be used.

Archivo in Figma intentionally substitutes for Proxima Nova on the live Squarespace site. Anton remains the heading family. Preserve the original vector wordmark. Approved focus component 17:7 supersedes legacy site outlines: three square strokes, Aubergine / pearl / Aubergine, static and unclipped; forced colors use the system outline.

## Native library mapping

Figma file: https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=87-2

| Pattern | Component set | Machine-facing purpose |
|---|---|---|
| Resources/Hero | 87:25 | Eyebrow, title, deck, sensory surface and frame; wide/stacked |
| Resources/FeaturedToolkitPanel | 87:45 | Featured toolkit, CTA and verification note; wide/stacked |
| Resources/TopicJumps | 87:74 | Six in-page topic links |
| Resources/ResourceRow | 87:173 | Kind, link title, external icon, description; light/inverse, wide/stacked, hover/focus |
| Resources/SystemPreviewCard | 87:214 | Contained 16:10 preview, kind, title, summary, visible credit |
| Resources/FigureCaption | 88:48 | Contextual figure, caption and attribution |
| Resources/ResourceGroup | 88:195 | Heading and resource list; optional figure and third/fourth/fifth rows |
| Resources/SystemShowcase | 88:280 | Four design-system references with licensing metadata |
| Resources/FeaturedResourcePair | 106:1103 | Equal-height Toolkit and System promos; two columns wide, stacked narrow |
| Shared header | 59:160 | Toolkit / Resources / Articles |
| Shared footer | 59:196 | Brand, Explore and Connect columns |

Wide assembly 88:281; narrow assembly 88:436. Both use linked instances and editable text. The assemblies include AI workflows, systems, Build & test, representation, motion resources and inclusive practice. Representation currently uses the reusable single-list group; the live two-column creator list remains a composition refinement.

## Component contract

Text properties use explicit names: Eyebrow, Title, Deck, Kind, Description, Caption, Heading, CTA and verification note where applicable. ResourceGroup exposes Show figure, Show third resource, Show fourth resource and Show fifth resource booleans. Do not detach instances to change copy. Keep visible labels and accessibility names consistent. Decorative external-link icons are hidden from assistive technology; the text link supplies the accessible name. The brand symbol must never substitute for an external-link icon.

Use actual anchors for destinations, not clickable divs. Keep one primary link per row/card; do not nest interactive controls. Use semantic section headings and lists. Topic jumps target stable section IDs; observed scroll-margin is 160px, to be verified against the actual sticky header. Never encode meaning solely in a kind color.

The header links Toolkit to its existing external toolkit destination, Resources to /designer-resources, System to /design-system, and Articles to /articles, in that order. Footer Explore: Articles, AI A11y Toolkit, Resources. Connect: Contact, Accessibility statement, About Dana Randall. Do not invent unknown hrefs.

## Layout and interaction

Observed content maximum 1320px; source breakpoint <=767px stacks columns. Standard group ratio 1:2 with 48px gap; resource row ratio 1:1.3 with 32px gap. Featured panel ratio 1:1.25, 48px gap, 40px padding; narrow padding 28px 24px. Preview grid two columns, 40px gap; narrow one column, 32px gap. Kind 12px uppercase, .09em tracking, padding 4px 8px. Icons 32px with 12px title gap.

Reuse approved finite card feedback: -3px, 140ms ease-out, no loop. Reduced motion and coarse pointers use the static state. Keep focus independent from hover. Source rows have a darker contextual shadow override than standard cards; reconcile in runtime before marking parity verified.

## Assets and sensory intent

Hero uses original DesignA11y sensory surface artwork. Other provider previews and instructional figures are labeled placeholders pending rights-cleared assets. Never redistribute Prime components, screens, screenshots or provider artwork without permission. References to Prime describe scope and licensing only. Publication requires replacing or removing these placeholders and checking credits.

Surfaces are continuous tactile fields serving sensory support, not isolated abstract objects. Smooth, rough, spiky, glossy, matte, velvet and sanded materials are permitted; encourage variety between assets. Preserve text clarity and quiet zones. Do not imply therapeutic outcomes.

## Acceptance and current limits

Wide and narrow Figma compositions were visually reviewed after reflow, with overlapping assembly positions and master grids corrected. Text families read back as Anton and Archivo. These are editable source-aligned drafts, not a pixel-perfect reproduction or tested production implementation.

Before verified/publication: exercise live narrow navigation, keyboard/focus, target sizing, contrast over artwork, long content, reduced motion/transparency and forced colors; resolve contextual shadows; complete exact representation grid, inverse gradient and featured backdrop treatment; replace rights-sensitive placeholders with publishable assets. Figma prototypes do not establish DOM semantics or screen-reader behavior.

## Optional motion skill references

Reviewed, not installed or adopted wholesale:
- https://www.figma.com/community/skill/41449/animation-asset-prep — useful for independent editable animation layers, retained instances and static resolved states.
- https://www.figma.com/community/skill/41506/ui-motion-choreography — useful for purpose, continuity and deliberate holds. Its spring, overshoot, camera and timing defaults do not override DesignA11y's restrained accessible motion contracts.
