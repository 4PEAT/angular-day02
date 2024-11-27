### Tasks for Practicing Angular Data Binding

#### **Task 1: Property Binding**
1. Update the text content of an `<h1>` element using the `title` property.
2. Create a button that displays `buttonText` as its label.
3. Use the `[disabled]` property to toggle whether the button is clickable based on the `isDisabled` property.

---

#### **Task 2: Event Binding**
1. Add a button that increments a `counter` property when clicked.
2. Display the current value of the counter using interpolation (`{{ counter }}`).

---

#### **Task 3: Combining Property and Event Binding**
1. Create a button that:
   - Is disabled based on the `isDisabled` property.
   - Toggles the `isDisabled` property when clicked.
2. Display a message below the button indicating whether it is enabled or disabled (e.g., "Button is Enabled/Disabled").

---

#### **Task 4: Two-Way Data Binding with `ngModel`**
1. Create an input field where users can enter their name.
2. Bind the input field to a `name` property using `ngModel`.
3. Display a greeting below the input field that updates dynamically as the user types (e.g., "Hello, [name]!").

---

#### **Task 5: Profile Form with `ngModel`**
1. Create a form with input fields for:
   - `name` (text input),
   - `age` (number input),
   - `city` (text input).
2. Use `ngModel` to bind these inputs to respective properties (`name`, `age`, and `city`).
3. Display the entered values dynamically in a profile summary below the form:
   - Show "Not provided" for any missing data.

---

#### **Extra Credit:**
1. Add validation for the form:
   - Ensure `name` is not empty.
   - Ensure `age` is a number greater than 0.
   - Provide feedback (e.g., "Age must be greater than 0") if validation fails.
2. Add a reset button to clear the form fields and reset the properties.

---
