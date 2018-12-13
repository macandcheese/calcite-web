<div class="panel panel-gray leader-1 trailer-1">
<svg xmlns='http://www.w3.org/2000/svg' class='svg-icon margin-right-half' height='24' width='24' viewBox='0 0 24 24'><path d='M11.5 1A10.5 10.5 0 1 0 22 11.5 10.499 10.499 0 0 0 11.5 1zm0 20.1a9.6 9.6 0 1 1 9.6-9.6 9.61 9.61 0 0 1-9.6 9.6zM11 6h1v7h-1zm.5 10.5a1 1 0 1 1 1-1 1.002 1.002 0 0 1-1 1z' /></svg>
<mark class='label label-blue margin-right-half'>Calcite Web 2.0 Update</mark>
<p class='leader-1 trailer-0 font-size--1'>
The HTML structure of modals has changed, please be sure to update your markup.
</p>
<p class='leader-half trailer-0 font-size--1'>
Distinct <em>modal-header</em>, <em>modal-footer</em>, and <em>modal-content</em> sections have been added to facilitate better spacing and placement of action buttons. It is recommended to place the main action button in a leading position within the footer.
</p>
</div>

Modals are meant to "take over" the screen and focus users attention on a dialog which presents the user with an opportunity to add, modify or create content. A modal should always be centered both vertically and horizontally within the browser window. When a modal is opened, the interface darkens and disables all other user interface elements in order to force a user to take an action required by their workflow. Two modals can't be open at once.

To create a link or button that opens a modal, you must add a `js-modal-toggle` class to the element, along with a `data-modal` attribute specifying the name of the modal that should open. The modal should also get a `data-modal` attribute with the same name.

Elements with the `js-modal-toggle` that are inside a modal don't need the `data-modal` attribute as they will just close the modal they are in.
