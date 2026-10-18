# Designer Resources — live-site parity audit

Contract ID: da.audit.designer-resources.v1
Source: https://www.design-a11y.com/designer-resources
Inspected: October 18, 2026 · live rendered DOM, screenshot, CSS rules and computed styles at 994px viewport
Status: partial alignment; page-specific parity NOT established

## Finding

The broad library expansion did not validate this page end to end. General foundations are present, but generic ResourceCard and ToolkitLanding are not faithful representations of its distinct patterns. Do not replace this page with those generic drafts or claim that Prime category coverage proves live-site parity. The live page is the source of observed site decisions; new proposals must remain distinguishable.

## Decision and gap matrix

| Live decision | System status | Required system work |
|---|---|---|
| Aubergine/Petal/Blush, Anton headings, Proxima Nova reading text | Brand anchors and headings present; Archivo difference intentional | Preserve documented platform mapping; measure reflow rather than silently changing live typography |
| Editorial hero: eyebrow, oversized heading and deck, sensory surface with frame/corner artwork to the side | Brand assets exist separately; composed resource hero absent | Build ResourceHero with wide/stacked arrangements, artwork purpose and protected text zone |
| Prominent AI A11y Toolkit panel before topic navigation | General toolkit prominence documented; generic card differs | Build FeaturedToolkitPanel: wide two-column layout, blush/pearl backdrop, detached corner, CTA and verification note |
| Six topic jump links | Generic navigation exists; resource topic-jump pattern absent | Named in-page navigation, wrapping links, target IDs and 160px observed scroll margin; test sticky header and focus |
| Editorial resource groups with section heading beside a list of resource rows | Generic ListItem too simple | ResourceGroup + ResourceRow: kind label, 32px icon, Anton link title, description, source/access metadata and separators |
| Dark editorial sections for AI workflows and representation | Dark token mode exists, but this composed local section treatment is missing | Explicit inverse-section composition with readable text, Blush accents, figures/captions and nested resources; observed gradient #442A42 to #291B29 is source-specific, not automatically a new approved UI token |
| Design-system preview cards with image, title, summary, licensing/access and credit | Generic ArticleCard and ResourceCard omit this anatomy | SystemPreviewCard: 16:10 contained preview, metadata, source credit, whole-card link and attribution/licensing handling; never redistribute provider previews without permission |
| Annotation and representation figures with captions and credit | No exact pattern | Figure/Caption/Credit composition, meaningful alt and context; retain attribution and image proportions |
| Shared finite shadow-lift feedback across resource rows and cards | General -3px/140ms card guidance exists | Map actual selectors and interaction scope; inherit shared approved focus. Page has a darker row-shadow override, requiring reconciliation with the generic Card lift style |
| Page header/footer destinations and arrangement | Generic headers/footer differ | Current header Toolkit / Resources / Articles and footer Explore/Connect groups need source-specific composition; generic templates are not site replicas |

## Observed layout rules (source evidence, not blanket token approval)

- Page content max-width 1320px; body 17.6px/29.04px at inspected viewport, Proxima Nova.
- Intro heading clamp(3.5rem, 7vw, 7rem); heading line-height 1.15. Intro width 60%; hero art width 35%, square.
- Featured toolkit panel columns 1fr/1.25fr, 48px gap, 40px padding. Mobile source breakpoint <=767px: one column, padding 28px 24px.
- Standard resource group columns 1fr/2fr, gap 48px; inner rows 1fr/1.3fr, gap 32px. Kind label precedes icon/title; icon 32px with 12px gap to title. Mobile source rules stack groups/rows.
- Kind label: 12px, uppercase, .09em tracking, 4px 8px padding, Aubergine on Blush.
- System preview grid: two columns, 40px gap; mobile one column, 32px gap. Preview media 16:10 with object-fit:contain; credits remain visible.
- Creator resource list: two columns, 32px/48px gaps; mobile one column.
- Resolved shared row shadow at inspection: 0 14px 30px rgba(16,12,20,.25), 0 3px 8px rgba(16,12,20,.15). Card shadow uses Aubergine alpha .12/.08. Transition 140ms ease-out. Decorative effects have contrast/transparency/forced-color handling in source.

## Important validation boundary

Mobile behavior above was read from source rules, not exercised at a mobile viewport. Hover/focus/preference behavior was inspected in CSS/computed resting state, not fully interactively tested. Older CSS declarations coexist with overrides; do not copy an early rule without resolving the cascade. The page contains legacy focus declarations; reconcile effective behavior against the approved triple-stroke focus contract rather than propagating old outlines.

## Acceptance before marking parity verified

Create the missing original compositions, compare desktop and narrow rendered layouts, preserve content and attribution, test actual hover/focus and in-page navigation, evaluate reduced motion/transparency and forced colors, then record source revision, Figma master IDs and evidence. Keep the live site unchanged during extraction. Never label a generic category match as page-level design validation.


## Alignment follow-up — October 18, 2026

Added eight original Resources component sets on page 87:2, wide assembly 88:281 and narrow assembly 88:436. Updated Header 59:160 and Footer 59:196 to core-site destinations and grouping. Added five resource color roles with explicit scopes, external-reference icons, optional figure and up to five resource rows. Reviewed wide/narrow screenshots and corrected overlapping masters/assemblies. Native Spec 96:1063 and docs/specs/resources-site-patterns.md record source authority and remaining limits.

This closes the absence of source-aligned native patterns; it does not establish full parity. Outstanding: exact representation two-column composition, inverse gradient and featured backdrop finish, publishable provider previews, live narrow/keyboard/preference/AT checks and contextual row-shadow reconciliation. Motion Lab layout excluded; no live-site changes.
