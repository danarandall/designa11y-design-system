# Editorial and resource content

Contract ID: da.content.v1 Owner: Dana Randall · October 18, 2026 Status: native component drafts; production behavior unimplemented/unvalidated

Original DesignA11y content patterns for inclusive design and AI. Neutral containers, clear hierarchy, controlled imagery and intentional whitespace. Sample pricing and review content is illustrative, not a live offering or testimonial.

## Content/ArticleCard

ID: da.content.article-card

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=61-33)

Purpose: Link to one editorial article with a clear title and reading context.

States: Default, Hover, Focus, Compact. Text properties: Category, Title, Summary, Metadata.

Semantics: Article with heading and one primary link; whole-card activation must not create duplicate tab stops. Decorative image empty alt when title gives context.

Keyboard: One primary article link; Enter follows; focus surrounds whole card.

Motion: Approved card-lift: -3px/140ms where appropriate; static reduced-motion/coarse-pointer feedback.

## Content/ResourceCard

ID: da.content.resource-card

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=61-62)

Purpose: Present a practical toolkit, guide or downloadable resource.

States: Default, Hover, Focus, Download. Text properties: Type, Title, Summary.

Semantics: Heading and descriptive link; download format/size explicit; avoid nested interactive card targets.

Keyboard: Separate actions only when necessary; clear order and focus.

Motion: contracts/motion/interface-microinteractions.json

## Content/FeaturedStory

ID: da.content.featured-story

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=61-79)

Purpose: Feature a single priority story without repeating it in the next article list.

States: Wide, Stacked. Text properties: Label, Title, Summary.

Semantics: Section with heading, summary and primary link; image purpose explicitly assigned.

Keyboard: Logical heading/link order; no duplicate links to same story within card.

Motion: contracts/motion/interface-microinteractions.json

## Content/AuthorProfile

ID: da.content.author

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=61-87)

Purpose: Identify article authors and provide relevant context.

States: Compact, Expanded. Text properties: Name, Role, Biography.

Semantics: Visible author name; adjacent avatar decorative; profile link has descriptive name.

Keyboard: Only profile/social links are tab stops.

Motion: contracts/motion/interface-microinteractions.json

## Content/Metadata

ID: da.content.metadata

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=61-92)

Purpose: Present date, reading time, format or revision consistently.

States: Article, Resource. Text properties: Metadata.

Semantics: Text and native time element with machine-readable datetime; format information belongs in link context.

Keyboard: Not focusable unless containing a meaningful category link.

Motion: contracts/motion/interface-microinteractions.json

## Content/Accordion

ID: da.content.accordion

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=61-118)

Purpose: Reveal optional supporting detail without hiding essential task instructions.

States: Collapsed, Expanded, Focus, Disabled. Text properties: Label, Content.

Semantics: Native details/summary or tested disclosure; button expanded/controls; heading level follows context.

Keyboard: Enter/Space toggles; Tab moves normally; no mandatory arrow model.

Motion: da.motion.disclosure; 160ms proposed measured-height transition, static alternative.

## Content/ListItem

ID: da.content.list-item

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=61-136)

Purpose: Present one resource, task or destination in a scan-friendly list.

States: Default, Hover, Focus, Selected. Text properties: Title, Description.

Semantics: List item containing a link, button or checkbox according to intent; avoid ambiguous clickable containers.

Keyboard: Native link/button/selection behavior, no custom listbox unless actual selection widget.

Motion: contracts/motion/interface-microinteractions.json

## Content/Quote

ID: da.content.quote

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=61-143)

Purpose: Separate quoted editorial content and attribution.

States: Quote, PullQuote. Text properties: Quote, Attribution.

Semantics: Blockquote with citation; no invented endorsement or testimonial.

Keyboard: Static text; citation link only if provided.

Motion: contracts/motion/interface-microinteractions.json

## Content/PricingCard

ID: da.content.pricing

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=61-164)

Purpose: Provide an optional access-plan pattern for future offerings, not a claim of a current paid product.

States: Standard, Featured, Unavailable. Text properties: Plan name, Price, Terms, Features.

Semantics: Heading, price and billing terms as text; descriptive action; no hidden recurring cost.

Keyboard: Native action/link; clear unavailable state.

Motion: contracts/motion/interface-microinteractions.json

## Content/Review

ID: da.content.review

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=61-172)

Purpose: Present verified resource feedback without inventing testimonials.

States: Summary, Detailed. Text properties: Rating, Review, Attribution.

Semantics: Review text, rating meaning and attribution; sample content must be replaced by verified feedback.

Keyboard: Only helpfulness/report actions are interactive.

Motion: contracts/motion/interface-microinteractions.json

## Content/ArticleBody

ID: da.content.article-body

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=61-183)

Purpose: Readable long-form editorial structure with headings and linked resources.

States: Default, Callout. Text properties: Heading, Body, Callout.

Semantics: Semantic article headings, paragraphs and lists; heading hierarchy follows page context.

Keyboard: Links in document order; no focusable body wrapper.

Motion: contracts/motion/interface-microinteractions.json

## Shared anatomy, tokens and layout

Semantic surface, text, action and border variables; shared Archivo type styles; space metrics and square radii. Named native layers and public text properties. Focus uses component 17:7, static triple stroke with 11px outset and 5px clear gap; never clip. Text wraps and height grows. Example widths are documentation examples, not fixed production widths. Intrinsic icons, grids and media proportions are intentional geometry.

## Implementation and evidence

Use native controls and tested headless primitives for complex patterns. Full AI A11y Toolkit reference/design.md is authoritative. Never treat drawings as keyboard or ARIA implementations. Do not improvise complex controls from these vectors. Implementation mapping: unassigned.

Before release: verify light/dark pairings and forced colors, keyboard/focus/announcements, 44px targets, 320px reflow and enlarged text, touch parity, interruption and reduced-motion alternatives, loading/error states and human review with named browser/AT pairings. Record evidence per component.

No Prime artwork, licensed components or code copied. Prime informed category breadth only. Existing live-site use is not a prerequisite for system inclusion.

<!-- Figma source: https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=61-272 · mirrored October 18, 2026 -->
