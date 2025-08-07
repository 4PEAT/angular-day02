

## Task 1: Stepper Component

**Component Name:** `app-stepper`

1. **Inputs**

   * **`initial`** (number): the starting value to display.
   * **`step`** (number): the amount to increment or decrement on each click.

2. **Display**

   * Show the current value between two buttons: a “–” button on the left and a “+” button on the right.

3. **Behavior**

   * When the user clicks the “+” button, add `step` to the current value.
   * When the user clicks the “–” button, subtract `step` from the current value.

4. **Output**

   * Expose an **`@Output()`** event called `valueChange` that emits the updated value (number) every time the user clicks either button.

5. **Parent Integration**

   * A parent component should be able to bind `[initial]` and `[step]` into `<app-stepper>`, and listen with `(valueChange)="…"` to keep its own counter in sync.

---

## Task 2: Todo Item Component

**Component Name:** `app-todo-item`

1. **Input**

   * **`todo`** (object) with properties:

     * `id` (number)
     * `text` (string)
     * `completed` (boolean)

2. **Display**

   * A checkbox that reflects `todo.completed`.
   * The `todo.text`, styled with a line-through if `completed` is true.
   * A “✕” button to delete the item.

3. **Behavior & Outputs**

   * When the user toggles the checkbox, emit an **`@Output()`** event `toggle` carrying the `todo.id`.
   * When the user clicks the delete button, emit an **`@Output()`** event `remove` carrying the `todo.id`.

4. **Parent Integration**

   * A parent component should be able to supply a list of todos via `*ngFor="let t of todos" [todo]="t"`, and bind `(toggle)` and `(remove)` handlers to update or remove items from its own `todos` array.

---

