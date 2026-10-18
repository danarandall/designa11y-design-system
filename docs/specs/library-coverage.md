# DesignA11y library coverage and Spec standard

Contract ID: da.system.coverage.v1 Owner: Dana Randall · Working plan · October 18, 2026

## Breadth and delivery matrix

Prime 6 informs breadth only. Do not copy or redistribute licensed assets. Components must express DesignA11y's inclusive design and AI context.

| **Family** | **Current coverage** | **Required expansion** |
|---|---|---|
| Foundations | Color, type, layout and focus drafts | Theme, responsive and runtime validation |
| Brand | Wordmark, symbol, favicon, frame, 3 surfaces | Usage, asset variety, export validation |
| Actions | Button, Link, Icon Button | Hierarchies, groups, destructive actions |
| Forms | Text Field plus Checkbox (12), Radio (8), Switch (8), Textarea (10) native drafts; Forms Spec 54:220 | Select, Combobox, Search, file input, validation and grouped forms; runtime validation |
| Navigation | Planned | Header, mobile navigation, tabs, breadcrumbs, pagination, menus |
| Editorial | Planned | Article/resource cards, featured story, author, metadata, tags, accordion |
| Feedback | Planned | Alert, toast, tooltip, progress, skeleton, empty/error states |
| Overlays | Planned | Dialog, drawer, popover; focus and keyboard models |
| Data and layout | Planned | Tables, lists, containers, grids, responsive section patterns |
| Motion foundations | Seam/Surface Field studies | Verified source mappings, playback/preferences, export checks |
| Live Motion Lab | Required; individual inventory pending | Demo container, control bar, instructions, individual demo patterns, motion behavior, static alternatives and preference states |
| Templates | Planned | Home, article, toolkit/resource, search/results and social/video |

## Motion Lab requirements

Preserve the live site's Motion Lab as part of the system. Keep card wrappers consistent and neutral; experimental visual variety belongs inside demonstrations. Inventory actual live demo names, controls and behavior before defining per-demo contracts. Document trigger, animated property, duration/easing or simulation behavior, bounds, stopping, replay, keyboard/touch equivalents, accessible instructions, preference handling and static state. Do not claim the Lab is represented merely because seam and Surface Field studies exist.

## Motion Lab → component microinteractions

Microinteractions are a first-class reusable part of the DesignA11y interface system, including patterns not yet used on the live site. Define behavior for real buttons, toggles, fields, cards, navigation, disclosures, feedback and overlays. The Motion Lab demonstrates and tests these behaviors; it does not restrict them to demo use. Existing site usage is provenance, not an inclusion requirement. New patterns may be proposed and built with explicit intent, parameters and validation status.

Record: component ID; Lab demonstration/source revision; purpose; trigger (hover, focus, press, selection or completion); animated properties; timing/easing or simulation parameters; interruption and reset; stopping behavior; pointer/touch/keyboard parity; reduced-motion alternative; static feedback; evidence status. Mark mappings proposed until the live example and implementation have been inspected. Focus indication itself stays static and unobscured. Persistent motion needs explicit playback behavior.

Known approved card feedback: restrained shadow lift, 140ms transition and -3px lift where appropriate; reduced motion and coarse pointer use static feedback. Keep experimental variety inside Lab demonstrations and preserve consistent card wrappers. For new interface patterns, author intentional parameters as proposals and validate them; do not present them as observed live-site values. Cover hover/press feedback, state transitions, selection, disclosure, validation, loading/completion, entry/exit and interruption. Reuse shared motion tokens where appropriate while allowing different behavior for different purposes.

## Delivery status model

Planned → native component draft → linked Spec → structural/visual review → runtime validation → release candidate. A visual variant does not prove interaction behavior. Record gaps component by component.

## Reusable component Spec template

1. Stable contract ID, owner, version, design and runtime status.
2. Purpose, appropriate uses and content context.
3. Master Figma link, Git contract path and implementation mapping (explicitly unmapped if absent).
4. Anatomy and stable layer names.
5. Public properties, defaults, allowed combinations and content rules.
6. Token bindings, typography, themes and dimensions.
7. States, transitions and combined focus/error/selection conditions.
8. Responsive behavior, text growth, localization and zoom.
9. Semantics, accessible name/role/state, descriptions and errors.
10. Keyboard, focus, pointer/touch, motion and preferences.
11. Acceptance criteria separating design evidence from runtime evidence.
12. Limitations and release restrictions.

## Retrieval

Read System contract, relevant component Spec, native component descriptions and full AI A11y Toolkit task references. Record versions. Prefer compatible instances. Never detach to bypass the public API. Verify retrieval with actual agent tasks before claiming measured machine efficiency.

## Expanded native library snapshot

67 additional component families and 232 authored variants were added in this build, plus 24 icons and 4 flag examples. Original components and IDs remain. These are native design drafts; scope parity is tracked by category, not identical licensed assets or variant counts.

### Forms

[Family Spec](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=58-844)

- Forms/Select: 5 variants, master 58:179
- Forms/Combobox: 6 variants, master 58:232
- Forms/Search: 4 variants, master 58:273
- Forms/DateField: 4 variants, master 58:306
- Forms/FileUpload: 4 variants, master 58:337
- Forms/Slider: 3 variants, master 58:363
- Forms/NumberStepper: 4 variants, master 58:393
- Forms/DatePicker: 3 variants, master 58:673

### Navigation

[Family Spec](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=59-278)

- Navigation/Item: 5 variants, master 59:18
- Navigation/Tabs: 4 variants, master 59:63
- Navigation/Breadcrumbs: 2 variants, master 59:68
- Navigation/Pagination: 3 variants, master 59:78
- Navigation/Menu: 3 variants, master 59:103
- Navigation/Header: 3 variants, master 59:160
- Navigation/Sidebar: 3 variants, master 59:183
- Navigation/Footer: 2 variants, master 59:196

### Feedback

[Family Spec](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=60-231)

- Feedback/Alert: 4 variants, master 60:19
- Feedback/Toast: 3 variants, master 60:31
- Feedback/Tooltip: 2 variants, master 60:36
- Feedback/Progress: 4 variants, master 60:58
- Feedback/Loading: 3 variants, master 60:66
- Feedback/Skeleton: 2 variants, master 60:76
- Feedback/EmptyState: 3 variants, master 60:92
- Feedback/ErrorState: 2 variants, master 60:103
- Content/Badge: 4 variants, master 60:112
- Content/Tag: 3 variants, master 60:126
- Content/Avatar: 3 variants, master 60:136
- Content/Rating: 3 variants, master 60:149

### Content

[Family Spec](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=61-272)

- Content/ArticleCard: 4 variants, master 61:33
- Content/ResourceCard: 4 variants, master 61:62
- Content/FeaturedStory: 2 variants, master 61:79
- Content/AuthorProfile: 2 variants, master 61:87
- Content/Metadata: 2 variants, master 61:92
- Content/Accordion: 4 variants, master 61:118
- Content/ListItem: 4 variants, master 61:136
- Content/Quote: 2 variants, master 61:143
- Content/PricingCard: 3 variants, master 61:164
- Content/Review: 2 variants, master 61:172
- Content/ArticleBody: 2 variants, master 61:183

### Actions

[Family Spec](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=62-152)

- Actions/ButtonSecondary: 12 variants, master 62:53
- Actions/ButtonTertiary: 12 variants, master 62:86
- Actions/ButtonDestructive: 12 variants, master 62:119

### Overlays

[Family Spec](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=63-176)

- Overlays/Dialog: 3 variants, master 63:25
- Overlays/Drawer: 3 variants, master 63:50
- Overlays/Popover: 2 variants, master 63:59
- Overlays/PreferenceBanner: 2 variants, master 63:74
- Actions/ButtonGroup: 2 variants, master 63:86
- Actions/SegmentedControl: 3 variants, master 63:115

### Data

[Family Spec](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=64-245)

- Data/TableCell: 4 variants, master 64:11
- Data/Table: 6 variants, master 64:117
- Data/DescriptionList: 2 variants, master 64:138
- Data/FilterBar: 3 variants, master 64:157
- Data/ResourceList: 3 variants, master 64:175

### Assets

[Family Spec](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=65-205)

- Assets/BrandMedia: 3 variants, master 65:30
- Assets/PaymentMethod: 3 variants, master 65:43
- Assets/LocaleOption: 4 variants, master 65:56
- Assets/DeviceTemplate: 3 variants, master 65:72
- Layout/Container: 3 variants, master 65:82
- Layout/Grid: 3 variants, master 65:110
- Layout/Divider: 2 variants, master 65:116
- Layout/SpacingReference: 3 variants, master 65:129

### Patterns

[Family Spec](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=68-456)

- Patterns/Homepage: 2 variants, master 68:110
- Patterns/Article: 2 variants, master 68:149
- Patterns/ToolkitLanding: 2 variants, master 68:184
- Patterns/SearchResults: 3 variants, master 68:239
- Patterns/PreferencesForm: 3 variants, master 68:278
- Patterns/MotionLab: 2 variants, master 68:303

## Remaining depth and release work

Category breadth is now represented by original drafts. Complete semantic building-block composition, extreme content/locale tests, theme and 320px checks, tested runtime primitive mapping, keyboard/AT evidence, individual interaction prototypes and final human review. Generic payment slots and neutral device frames are intentional original alternatives to licensed provider/device artwork. Country flags are illustrative examples, not an exhaustive country asset pack. Pricing/review content is sample-only. Never equate component count with accessibility or production readiness.

<!-- Figma source: https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=52-8 · mirrored October 18, 2026 -->
