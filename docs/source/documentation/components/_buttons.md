<div class="panel panel-gray leader-1 trailer-1">
<mark class='label label-blue'>Calcite Web 2.0 Update</mark>
<p class='leader-half trailer-0 font-size--1'>
This update contains new button styles, and updates existing ones to ensure consistency across interfaces. More options for using red as an indication of a destructive action have been added.
</p>
<p class='leader-half trailer-0 font-size--1'>

`btn-green` has been deprecated. Green should not be used for buttons or call to actions.

`btn-white` has been renamed `btn-light`.
</p>
</div>

Buttons are created by adding a class of `btn` to either a `<button>` or `<a>` element. `btn-{color}` classes can be mixed with `btn-{scale}` classes.

```html
<a href="#" class="btn">Link that looks like a Button</a>
<button class="btn">Button</button>
<button class="btn btn-red">Red Button</button>
```

<h4 id="button-links">Button Links</h4>

Sometimes, the proper semantic element is a button, but you would rather the element look more like a link. In these instances, Calcite Web provides an alternate class `btn-link` which styles a button element as if it were a simple anchor:

<button class="btn-link">This is a button</button>

The `btn-link` class also allows you to style inline anchors you wish to receive an underline animation. Here's <a class="btn-link">an example of a btn-link</a> within a block of text that may wrap.

```html
<button class="btn-link">This is a button</button>
Here's <a class="btn-link">an example of a btn-link</a> within a block of text that may wrap.
```
