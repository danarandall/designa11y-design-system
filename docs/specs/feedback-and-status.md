# Feedback and status

Contract ID: da.feedback.v1 Owner: Dana Randall · October 18, 2026 Status: native component drafts; production behavior unimplemented/unvalidated

Explicit messages, steady loading states and meaningful recovery. All severity and selection meanings have textual equivalents; motion is optional and separately specified.

## Feedback/Alert

ID: da.feedback.alert

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=60-19)

Purpose: Persistent contextual feedback with explicit meaning.

States: Information, Success, Warning, Error. Text properties: Title, Message.

Semantics: Status or alert only when dynamically appropriate; static alert panels need no live role. Severity is named in text, not color alone.

Keyboard: Text is not focusable; actions and dismiss buttons are.

Motion: contracts/motion/interface-microinteractions.json

## Feedback/Toast

ID: da.feedback.toast

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=60-31)

Purpose: Nonblocking outcome notification without losing task context.

States: Information, Success, ActionRequired. Text properties: Message. Heading follows state.

Semantics: Tested notification region; polite status by default; persistent if action required; no essential timed-only content.

Keyboard: Do not steal focus; actionable notifications have discoverable controls and enough time.

Motion: contracts/motion/interface-microinteractions.json

## Feedback/Tooltip

ID: da.feedback.tooltip

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=60-36)

Purpose: Supplement a clear control label with brief nonessential help.

States: Above, Below. Text properties: Content.

Semantics: Tested tooltip; role=tooltip associated through describedby; no interactive content.

Keyboard: Shown on focus and hover; Escape dismisses; remains while pointer is over it; never sole accessible name.

Motion: contracts/motion/interface-microinteractions.json

## Feedback/Progress

ID: da.feedback.progress

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=60-58)

Purpose: Communicate measurable completion without animation dependence.

States: Start, InProgress, Complete, Error. Text properties: Label.

Semantics: Native progress with accessible label and known max/value; omit numeric value if unknown; error is textual.

Keyboard: Not focusable unless it contains an action; status announcements throttled.

Motion: contracts/motion/interface-microinteractions.json

## Feedback/Loading

ID: da.feedback.loading

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=60-66)

Purpose: Give a stable pending-operation status and completion feedback.

States: Inline, Block, Complete. Text properties: none; status follows state.

Semantics: Named status; aria-busy on affected region; avoid repeated announcements.

Keyboard: Do not move focus or disable unrelated controls; cancellation if operation warrants.

Motion: contracts/motion/interface-microinteractions.json

## Feedback/Skeleton

ID: da.feedback.skeleton

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=60-76)

Purpose: Reserve content geometry during loading without visual noise.

States: Card, List. Text properties: .

Semantics: Decorative aria-hidden skeleton; one adjacent loading status. Static by default.

Keyboard: Never focusable; no fake interactive controls.

Motion: contracts/motion/interface-microinteractions.json

## Feedback/EmptyState

ID: da.feedback.empty-state

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=60-92)

Purpose: Explain absence of content and a useful next action.

States: NoResults, NoSavedItems, FirstUse. Text properties: none; state-specific content is fixed.

Semantics: Heading and explanation; no live-region by default; avoid blame and decorative over-explanation.

Keyboard: Clear next action in reading order.

Motion: contracts/motion/interface-microinteractions.json

## Feedback/ErrorState

ID: da.feedback.error-state

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=60-103)

Purpose: Explain a failed task with recovery and preserved input.

States: Recoverable, Unavailable. Text properties: Title, Message.

Semantics: Visible heading/message; alert only for newly occurring urgent errors; accessible recovery link/button.

Keyboard: Focus remains logical; failed submit may focus error summary; never discard entered content.

Motion: contracts/motion/interface-microinteractions.json

## Content/Badge

ID: da.content.badge

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=60-112)

Purpose: Compact noninteractive category or status label.

States: Neutral, New, Updated, ReviewPending. Text properties: Label.

Semantics: Plain text; never rely on color; not a button.

Keyboard: Not a tab stop.

Motion: contracts/motion/interface-microinteractions.json

## Content/Tag

ID: da.content.tag

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=60-126)

Purpose: Represent a topic or chosen filter.

States: Static, Removable, Selected. Text properties: Label.

Semantics: Static text, link or named toggle according to use; remove button includes tag name.

Keyboard: Interactive tag Enter/Space per role; remove is a distinct named action.

Motion: contracts/motion/interface-microinteractions.json

## Content/Avatar

ID: da.content.avatar

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=60-136)

Purpose: Represent an author or contributor without requiring a photo.

States: Initials, Anonymous, Group. Text properties: Name.

Semantics: If adjacent name is present, decorative; otherwise meaningful name equivalent. Never infer identity from image.

Keyboard: Not focusable unless a separate profile link.

Motion: contracts/motion/interface-microinteractions.json

## Content/Rating

ID: da.content.rating

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=60-149)

Purpose: Collect helpfulness feedback, never an accessibility conformance score.

States: ReadOnly, Interactive, Rated. Text properties: Question.

Semantics: Read-only text summary or tested radio group with each value named; do not use icon color as sole value.

Keyboard: Radio group arrows and Space; visible labels for choices; submit if required.

Motion: contracts/motion/interface-microinteractions.json

## State-specific content API

State-specific EmptyState headings/messages, Loading status and Toast headings are fixed semantic defaults. They do not expose generic text properties that could silently overwrite another state. Badge Label applies to Neutral; New, Updated and ReviewPending retain explicit fixed status text. For final public properties, read the native master API and the reconciled component lists above.

## Shared anatomy, tokens and layout

Semantic surface, text, action and border variables; shared Archivo type styles; space metrics and square radii. Named native layers and public text properties. Focus uses component 17:7, static triple stroke with 11px outset and 5px clear gap; never clip. Text wraps and height grows. Example widths are documentation examples, not fixed production widths. Intrinsic icons, grids and media proportions are intentional geometry.

## Implementation and evidence

Use native controls and tested headless primitives for complex patterns. Full AI A11y Toolkit reference/design.md is authoritative. Never treat drawings as keyboard or ARIA implementations. Do not improvise complex controls from these vectors. Implementation mapping: unassigned.

Before release: verify light/dark pairings and forced colors, keyboard/focus/announcements, 44px targets, 320px reflow and enlarged text, touch parity, interruption and reduced-motion alternatives, loading/error states and human review with named browser/AT pairings. Record evidence per component.

No Prime artwork, licensed components or code copied. Prime informed category breadth only. Existing live-site use is not a prerequisite for system inclusion.
