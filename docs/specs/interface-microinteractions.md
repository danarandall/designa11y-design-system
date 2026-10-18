# Interface microinteractions

Contract ID: da.motion.microinteractions.v1 Owner: Dana Randall · October 18, 2026 Status: authored proposals except approved card lift; runtime validation pending

## Scope

Reusable behavior for the real interface, including patterns not yet used on the live site. Motion Lab demonstrates, evaluates and tests these patterns. It is not the boundary of their use. Keep a library of intentional recipes, not just isolated motion demos.

## Selection and accessibility

For each application evaluate benefit/purpose, frequency, speed/interruption, function/readability and sensory impact. No requirement to animate every element. State and semantics update immediately. Motion never blocks activation or focus. Focus indication remains static. Reduced motion may be completely static; do not require residual movement. Preserve equivalent information for keyboard, touch and pointer. Provide stopping/control for persistent motion and avoid unintended looping.

## Recipe catalog

| **ID** | **Interface use** | **Authored parameters** | **Alternative / status** |
|---|---|---|---|
| card-lift | Article/resource cards | -3px, 140ms ease-out, approved shadow | Static feedback for reduced motion/coarse pointer; approved design |
| action-feedback | Button hover/press | Fill/border 120ms ease-out; no spatial motion | Immediate state change; proposal |
| selection-change | Checkbox/radio selection | Indicator opacity 100ms ease-out | Immediate mark; proposal |
| switch-change | Switch toggle | Thumb travels 16px, 140ms ease-out, no overshoot | Immediate position/state; proposal |
| disclosure | Accordion expansion | Measured height, 160ms ease-out; chevron 90deg | Immediate open/close; proposal |
| feedback-reveal | Inline validation/completion | Opacity 120ms ease-out; no shake or displacement | Immediate message; proposal |
| overlay | Dialog/popover open/close | Opacity 140ms ease-out | Immediate appearance; proposal |
| loading | Pending action/progress | Static progress text by default; loop requires its own spec | Static status; proposal |

## Interruption and implementation

Retarget from current values. Reverse promptly; do not queue animations after rapid input. Cancel stale completion handlers. Disclosure content visibility and focus follow semantic state; overlay focus management never waits for animation. Progress stops on success, error or cancellation. Never animate all CSS properties. Recipe parameters are portable intent; choose implementation techniques appropriate to the property and runtime.

## Evidence and links

[Machine contract](https://github.com/danarandall/designa11y-design-system/blob/main/contracts/motion/interface-microinteractions.json). Native timeline studies now exist at 67:89 for card lift, switch thumb travel, checkbox selection and inline feedback, with static comparison states. They demonstrate authored transitions, not production input handling or automated preference detection. Runtime interruption, keyboard/touch equivalence, preferences and human review remain pending. Video export verification is not claimed.

## External evaluation reference

[Emil Kowalski — find-animation-opportunities](https://github.com/emilkowalski/skills/blob/main/skills/find-animation-opportunities/SKILL.md), reviewed October 18, 2026. Its opportunity-filter approach is useful. It is not installed or adopted wholesale. DesignA11y adds explicit sensory review and static alternatives; full AI A11y Toolkit and Dana's decisions retain authority. Do not adopt hold-to-confirm or fixed input-modality exclusions without an appropriate interaction design.
