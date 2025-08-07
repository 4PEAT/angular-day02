**Requirements: Child→Parent Text Input**

1. **Child Component (`ChildMessageInputComponent`)**

   * Expose an **input field** (`<input>`) bound to a component property (e.g. `inputText`).
   * Provide a **“Send”** button that, when clicked, emits an event carrying the current `inputText`.
   * Declare an `@Output()` EventEmitter<string> (e.g. `message`) and call `emit(inputText)` in the send handler.
   * (Optional) Clear the input field after emitting.

2. **Parent Component (`ParentComponent`)**

   * Include the child selector `<app-child-message-input>` in its template.
   * Bind to the child’s output event: `(message)="onMessageReceived($event)"`.
   * Implement the `onMessageReceived(text: string)` method to store the incoming text in a property (e.g. `childMessage`).
   * Display the stored `childMessage` in the parent’s template via interpolation (`{{ childMessage }}`).



**Requirements: Parent→Child Favorite Star Display**

1. **Child Component (`FavoriteStarComponent`)**

   * Declare an `@Input()` property named `isFavorite` of type `boolean`.
   * In its template, display a filled star when `isFavorite` is `true`, or an outlined star when `false`.

2. **Parent Component (`ParentComponent`)**

   * Define a `favoriteFlag: boolean` property initialized to `false`.
   * In its template:

     * Include a checkbox or toggle control bound via `[(ngModel)]="favoriteFlag"`.
     * Render `<app-favorite-star>` with `[isFavorite]="favoriteFlag"` so that the child updates as the flag changes.


   * Import `FormsModule` to enable two-way binding on the parent’s checkbox/toggle.
   * Declare `FavoriteStarComponent` in the module’s `declarations`.
