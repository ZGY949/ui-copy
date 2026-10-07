---
name: ui-copy
description: "Reduce excessive descriptive and explanatory text when building, revising, or reviewing websites, apps, mini programs, and admin interfaces. Decide whether to remove text, shorten it to a familiar word or phrase, put it in the right place, or turn it into a working control or lightweight interaction. Use for UI copy, information placement, and interaction simplification; not for long-form marketing, educational content, color-only changes, or backend development."
license: MIT
---

# UI Copy

Address the tendency of AI-built pages to explain features, guide actions, and fill empty states with long paragraphs. Put necessary information where people need it, using titles, labels, states, and working interactions to keep the page clear and uncluttered.

## Start with the page task and the information's role

- Inspect the relevant page, screenshot, design, or code. Identify the task, what existing titles, data, controls, and states already express, and which explanations still provide independent value.
- Separate interface guidance from the content itself. Locations, dates, counts, user text, articles, and educational content are not redundant hints to remove.
- Follow the product's terminology, target language, and visual system. Clear hierarchy, appropriate placement, and restrained density create a refined interface; unfamiliar words, tiny type, and obscure gestures do not.
- Work within the authorized scope. A review produces suggestions, a single-string edit focuses on that string, and page implementation or broader optimization can address related structure and lightweight interactions. Proceed directly with clear, local changes.

## Four approaches: remove, shorten, place, interact

Choose according to the role of the text. Combine approaches when useful; do not force every sentence through a fixed procedure.

**Remove repetition.** Delete sentences that restate what a title, button, data, or current state already shows, including empty welcomes, feature slogans, and gestures such as "click below." The change is valid only if people can still find the action and complete the task.

**Shorten wording.** Use a familiar word or phrase when it expresses the same meaning. Titles name objects, controls name actions, and short labels show states. Keep the object and meaning clear instead of enforcing a fixed word count.

**Put information in place.** Put names in titles, input requirements beside fields, states beside their objects or results, errors where they occur, and consequences before the decision. Occasional help can use a clear link, disclosure, or detail view.

**Turn explanations into interactions.** When text explains how to search, filter, switch, sort, add, or recover, prefer a visible, usable control. Search inputs, filters, view controls, sorting handles, empty-state actions, and recovery actions can express what people can do without repeated instructions.

See [examples and prerequisites](references/patterns.en.md). For English labels and phrases, read [English wording](references/en.md) when needed.

## Make the interaction do the work

- Check the existing capability, data, and business action first. If an available action is buried in explanatory text, expose it and place it more directly.
- When page implementation or interaction optimization is authorized, reuse existing data, components, and business capabilities for local, reversible changes. For example, implement status filtering when the list already has status data, rather than drawing three decorative labels.
- Controls need real behavior and feedback: a selection changes the corresponding content, an empty-state action starts the relevant flow, and recovery performs the existing recovery action. Selection, disabled conditions, loading, and results should be understandable.
- If only copy changes or analysis are authorized, describe interaction changes as specific recommendations. Follow task and project boundaries for new business rules, external services, permissions, costs, or an unclear implementation scope.
- Do not invent a capability to eliminate text. If implementation prerequisites are unknown, explain them and the changes required. A diagram, button appearance, or prototype does not prove a working product capability.
- Verify discoverability and use with the supported input methods. Touch cannot depend on hover, and icon-only controls retain accessible names. A help action must remain clear after the paragraph moves behind it.

## Keep necessary information clear

Present costs, permissions, irreversible consequences, unsaved data, important limits, and failure recovery clearly at the appropriate time. Do not hide them until after a decision just to reduce the word count.

Occasional help may be disclosed on demand. Information required for the main task remains visible in context. Do not add a question mark, hint card, or disclosure to every heading and create a different kind of clutter. For genuinely complex flows, provide short guidance at each step and retain a full explanation when necessary.

Write from real states and capabilities. Do not declare success or failure when the outcome is unknown, or promise safe retries or no data loss without evidence. Handle user and third-party text according to its actual source.

## Verify and deliver

Check the text, placement, and interactions affected by the change:

- Can people identify the object and see their next action without reading a paragraph about an obvious feature?
- Do titles, labels, controls, and states each serve a purpose? Does repeated guidance still occupy the main action area?
- Do changed controls work? Do selection, cancellation, empty states, and feedback match the underlying behavior?
- Do necessary notices appear before the decision? Do narrow layouts, long names, or the target language cause critical information to wrap or truncate?

Preserve unaffected data, business rules, and calling conventions when changing code. Follow the project's implementation and validation rules. If only text, source, or screenshots were available, state that scope rather than claiming interaction or device verification.

For one issue, give the revision and its reason directly. For a batch review, you can list the location, original text, chosen approach, replacement, and implementation status or prerequisite. Distinguish implemented interactions from recommendations. Explain what changed, how it was checked, and what remains unverified.

Read [source notes](references/sources.en.md) when tracing the general writing references. Sources support judgment; they do not replace product facts or explicit task requirements.
