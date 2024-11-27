### Tasks for Angular Data Binding and Directives Practice

#### **Task 1: Property Binding**
1. Create an `<h1>` element that displays a title using the `[textContent]` property.
   - Use the `title` property from the component (`title = 'Angular Binding Example';`).
2. Create a button that:
   - Displays the `buttonText` property as its label.
   - Is disabled based on the `isDisabled` property (`[disabled]="isDisabled"`).

---

#### **Task 2: Event Binding**
1. Add a button labeled "Increment Counter" that:
   - Calls the `incrementCounter()` method on click.
   - Updates the `counter` property.
2. Display the value of the `counter` below the button using interpolation.

---

#### **Task 3: Combining Property and Event Binding**
1. Add a button that:
   - Is disabled if `isDisabled` is true (`[disabled]="isDisabled"`).
   - Calls the `toggleButtonState()` method to toggle the `isDisabled` property.
2. Show a message below the button indicating whether it is enabled or disabled using:
   - A message like: **"Button is Enabled/Disabled"**.

---

#### **Task 4: Two-Way Data Binding (`ngModel`)**
1. Add an input field for the user to enter their name.
   - Bind it to the `name` property using `[(ngModel)]`.
2. Display a greeting below the input field that updates dynamically:
   - Example: **"Hello, [name]!**" or **"Hello, Guest!"** if the name field is empty.

---

#### **Task 5: Binding Multiple Properties in a Profile Form**
1. Create a form with input fields for:
   - **Name** (`name` property).
   - **Age** (`age` property).
   - **City** (`city` property).
2. Use `[(ngModel)]` for two-way data binding.
3. Display the profile details dynamically:
   - Show "Not provided" if any field is left empty.

---

#### **Task 6: Structural Directives**
1. Use `*ngIf` to conditionally display messages based on the `counter` value:
   - Show **"The Counter is Positive!"** if the `counter > 0`.
   - Show **"The Counter is Zero"** if `counter === 0`.
   - Show **"The Counter is Negative!"** if `counter < 0`.

2. Use `*ngFor` to display a list of tasks stored in the `tasks` array.
   - Show the task index and description dynamically.
   - Example: **"1. Task A"**, **"2. Task B"**.

---

#### **Task 7: Attribute Directives**
1. Use `[ngClass]` to apply CSS classes based on the `counter` value:
   - Add the class `positive` if `counter > 0`.
   - Add the class `negative` if `counter < 0`.
   - Add the class `neutral` if `counter === 0`.

2. Use `[ngStyle]` to dynamically change the text color:
   - Use green if `counter > 0`.
   - Use red if `counter < 0`.
   - Use black if `counter === 0`.

---

#### **Task 8: Counter Buttons**
1. Add three buttons to manipulate the `counter`:
   - Increment: Calls `incrementCounter()` and increases the counter by 1.
   - Decrement: Calls `decrementCounter()` and decreases the counter by 1.
   - Reset: Calls `resetCounter()` and sets the counter to 0.

---

#### **Task 9: Add Tasks**
1. Add an input field and button for task management:
   - Bind the input field to the `newTask` property using `[(ngModel)]`.
   - On button click, add the task to the `tasks` array using the `addTask()` method.
2. Display a message like **"No tasks available"** if the `tasks` array is empty (use `*ngIf`).

---
