# Examples for handling explanations

Choose an approach for descriptive and explanatory UI text. These are design and implementation examples; check the real task, capabilities, and authorized scope before applying them.

## 1. Turn a long sentence into a title or phrase

**Original explanation**

> Here, you can view and manage all the projects you have created.

**Presentation**

Use My projects as the page title and show the project list below it. When the title and list already identify the object, remove the repeated introduction. There is no need to add "Welcome to project management."

Titles identify objects; buttons express actions, such as New project, Filter, and Sort. Do not rewrite the same feature introduction and place copies beside the heading, card, and button.

## 2. Turn an instruction into a working control

**Original explanation**

> You can filter the project list by status to see projects in progress or completed.

**Presentation**

Provide All / In progress / Completed filters beside the list and make the current selection clear.

**Prerequisites and implementation**

- If status data exists and the task authorizes page implementation or interaction changes, implement local filtering with existing data and components.
- A selection must actually update the list. Check the filtered empty state and the action to clear the selection or return to All.
- Remove the original instructions once the controls express the action. A short label can still show a necessary filter condition or current scope.
- If only copy editing is authorized, recommend the specific filter area. If a capability is missing, explain the required change instead of inventing a working feature.

The same judgment applies to search inputs, view switches, sorting, and editing actions. Each control must produce real behavior rather than only change its appearance.

## 3. Give an empty state a clear status and direct action

**Original explanation**

> You do not have any projects yet. Click the button below to create your first project. Once created, you can view and manage it here.

**Presentation**

No projects yet, with a New project button.

When page changes are authorized and a creation flow already exists, connect the button to that real flow. The state and action are enough to continue; do not add a paragraph explaining the button.

For a search with no results, show the actual result and an available action to adjust the query or clear filters. A loading failure needs an error and recovery path; it cannot be presented as No projects yet. A quiet state with nothing to do does not always need a creation action.

## 4. Put information beside what it describes

| Information's role | Better location and form |
|---|---|
| Identify what to enter | A field label, rather than only a placeholder that disappears |
| Show an example or format | A short placeholder or nearby hint |
| Explain a real required field, count, or format limit | A short hint visible before entry; an actionable error at the field |
| Describe an object's current state | A state label beside the object or in the result area |
| Explain a term only some people need | A clear Help action, disclosure, or detail view |
| Describe costs, permissions, or irreversible consequences | The action area, confirmation, or notice before the decision |

For example, remove "Please enter a project name below" from the top of the form and provide a Project name label at the field. Add a nearby requirement only when the real limit needs to be known in advance.

Match help to the input method: touch interfaces cannot rely only on hover tooltips. Do not hide information needed for a decision behind help, or add an explanation card to every field.

## 5. A long explanation may reveal an action or flow problem

> Click the icon in the upper-right corner to open the filter panel, then select a status.

Inspect the action first. Is the icon understandable? Is filtering common enough to deserve a visible Filter button or an open filter area? Remove the tutorial if the entry point is already clear. If an interaction needs changing, implement and verify it within the task's scope.

Similarly, removing "Press and hold here to sort" must not leave only a hidden gesture. Provide a clear sorting action, handle, or discoverable operation suited to the platform. Verify native gesture behavior on the target platform when it matters.

## 6. Explanations that should remain

- Permanent deletion, costs, permissions, and data effects need truthful consequences before the decision.
- Unusual input or business constraints need a short hint that helps people complete the task.
- Failure recovery needs a specific, usable action, rather than just "Something went wrong."
- First use or a complex flow may need guidance at each step; do not keep a complete tutorial on every frequently used page.
- Articles, course material, user-written text, and task data such as locations, dates, and counts follow their own content purpose.

A simpler page comes from text, placement, and interactions each doing their job. If removing words makes the page harder to understand, forces guessing, or leaves controls that only look usable, the original problem has not been solved.
