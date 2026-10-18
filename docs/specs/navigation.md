# Navigation systems

Contract ID: da.navigation.v1 Owner: Dana Randall · October 18, 2026 Status: native component drafts; production behavior unimplemented/unvalidated

Navigation for editorial resources, toolkit guidance and Motion Lab. Preserve consistent naming, destinations and keyboard models across layouts.

## Navigation/Item

ID: da.navigation.item

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=59-18)

Purpose: Reusable labelled navigation destination.

States: Default, Hover, Focus, Current, Disabled. Text properties: Label.

Semantics: Anchor for route changes; aria-current=page for current destination.

Keyboard: Tab to link; Enter follows; do not use arrow keys for plain navigation.

Motion: contracts/motion/interface-microinteractions.json

## Navigation/Tabs

ID: da.navigation.tabs

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=59-63)

Purpose: Switch between related panels in one context.

States: FirstSelected, SecondSelected, Focus, Disabled. Text properties: Panel content.

Semantics: Tested tabs primitive with tablist, tabs, selected state and labelled panels.

Keyboard: Roving tab stop; Left/Right arrows, Home/End; manual activation if content is slow.

Motion: contracts/motion/interface-microinteractions.json

## Navigation/Breadcrumbs

ID: da.navigation.breadcrumbs

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=59-68)

Purpose: Show hierarchy and provide ancestor navigation.

States: Default, Compact. Breadcrumb items are separate named layers; edit destinations and labels together in the consuming composition. No flattened Trail property.

Semantics: Labelled breadcrumb nav with ordered list; final item aria-current=page.

Keyboard: Only ancestor links are tab stops; compact overflow has a named control.

Motion: contracts/motion/interface-microinteractions.json

## Navigation/Pagination

ID: da.navigation.pagination

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=59-78)

Purpose: Move through bounded result pages with clear current state.

States: FirstPage, MiddlePage, LastPage. Text properties: Summary.

Semantics: Labelled pagination nav; links for destinations; aria-current=page; disabled previous/next not actionable.

Keyboard: Tab through available links; Enter follows. No custom arrow navigation.

Motion: contracts/motion/interface-microinteractions.json

## Navigation/Menu

ID: da.navigation.menu

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=59-103)

Purpose: Offer a short contextual action list.

States: Default, ItemFocus, ItemDisabled. Text properties: .

Semantics: Tested menu/menuitem primitive for actions; ordinary destination lists should remain links.

Keyboard: Trigger Enter/Space opens; arrows, Home/End; Escape closes and restores trigger focus.

Motion: contracts/motion/interface-microinteractions.json

## Navigation/Header

ID: da.navigation.header

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=59-160)

Purpose: Consistent DesignA11y site identity, primary destinations and mobile menu. Core-site destinations are Toolkit, Resources, System and Articles, in that order. System links to /design-system. Motion Lab is excluded as a layout reference during this alignment pass.

States: Desktop, Compact, MenuOpen. Text properties: .

Semantics: Header landmark, home link, labelled primary nav; compact disclosure button with expanded/controls.

Keyboard: Tab links; menu button Enter/Space; Escape closes disclosure and returns focus; no desktop menubar role.

Motion: contracts/motion/interface-microinteractions.json

## Navigation/Sidebar

ID: da.navigation.sidebar

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=59-183)

Purpose: Navigate resource and documentation sections.

States: Default, SectionExpanded, Compact. Text properties: Title.

Semantics: Named navigation landmark with links and optional disclosure sections; current page indicated.

Keyboard: Tab links/disclosures; Enter/Space toggles section; no tree role unless full tree pattern implemented.

Motion: contracts/motion/interface-microinteractions.json

## Navigation/Footer

ID: da.navigation.footer

[Master](https://www.figma.com/design/YnhNUlEByax6x6ZY1YQL9e/DesignA11y-Design-System?node-id=59-196)

Purpose: Consistent secondary navigation, brand context and legal links.

States: Desktop, Stacked. Fixed brand tagline and separately editable native navigation labels; the obsolete flattened Description property was removed during source alignment. Explore contains Articles, AI A11y Toolkit and Resources. Connect contains Contact, Accessibility statement and About Dana Randall.

Semantics: Footer landmark; separately named nav groups; descriptive link text.

Keyboard: Normal link order follows visual and document order.

Motion: contracts/motion/interface-microinteractions.json

## Shared anatomy, tokens and layout

Semantic surface, text, action and border variables; shared Archivo type styles; space metrics and square radii. Named native layers and public text properties. Focus uses component 17:7, static triple stroke with 11px outset and 5px clear gap; never clip. Text wraps and height grows. Example widths are documentation examples, not fixed production widths. Intrinsic icons, grids and media proportions are intentional geometry.

## Implementation and evidence

Use native controls and tested headless primitives for complex patterns. Full AI A11y Toolkit reference/design.md is authoritative. Never treat drawings as keyboard or ARIA implementations. Do not improvise complex controls from these vectors. Implementation mapping: unassigned.

Before release: verify light/dark pairings and forced colors, keyboard/focus/announcements, 44px targets, 320px reflow and enlarged text, touch parity, interruption and reduced-motion alternatives, loading/error states and human review with named browser/AT pairings. Record evidence per component.

No Prime artwork, licensed components or code copied. Prime informed category breadth only. Existing live-site use is not a prerequisite for system inclusion.
