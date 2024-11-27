### Tasks for Student Management Application

#### **Task 1: Display Student List**
1. Use a `<table>` to display the list of students.
2. Show the following details for each student:
   - **ID**
   - **Name**
   - **Email**
3. Use `*ngFor` to iterate over the `students` array and populate the table rows dynamically.

---

#### **Task 2: Add New Student**
1. Create a form for adding a new student with the following input fields:
   - **ID** (number)
   - **Name** (text)
   - **Email** (text)
2. Bind the input fields to a `newStudent` object using `ngModel`.
3. Add a **Submit** button that calls the `addStudent()` method when clicked.
4. Ensure that:
   - All fields are required.
   - A new student is added to the `students` list only when all fields are filled.

---

#### **Task 3: Reset Form After Adding**
1. After a new student is added, clear the form fields by resetting the `newStudent` object.
   - Example: `this.newStudent = { id: 0, name: '', email: '' };`.

---

#### **Task 4: Validate Unique Student ID**
1. Before adding a new student, check if the `id` already exists in the `students` list.
2. If a duplicate ID is found:
   - Show an alert: "A student with this ID already exists!".
   - Prevent adding the student.

---

#### **Task 5: Use Interpolation**
1. Add a heading that dynamically displays the total number of students.
   - Example: **"Total Students: {{ students.length }}"**.

---

#### **Task 6: Highlight Empty Fields**
1. Use the `required` attribute to mark fields as mandatory.
2. Show a message (e.g., "All fields are required!") if the form is submitted with empty fields.

---

### Bonus Tasks

#### **Task 7: Add Edit Functionality**
1. Add an "Edit" button in each table row.
2. When clicked, populate the form fields with the selected student’s details for editing.
3. Update the student record when the form is submitted.

#### **Task 8: Add Delete Functionality**
1. Add a "Delete" button in each table row.
2. When clicked, remove the student from the `students` list.

