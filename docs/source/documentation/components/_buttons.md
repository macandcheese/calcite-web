<div class="panel panel-gray leader-1 trailer-1">
<svg xmlns='http://www.w3.org/2000/svg' class='svg-icon margin-right-half' height='24' width='24' viewBox='0 0 24 24'><path d='M11.5 1A10.5 10.5 0 1 0 22 11.5 10.499 10.499 0 0 0 11.5 1zm0 20.1a9.6 9.6 0 1 1 9.6-9.6 9.61 9.61 0 0 1-9.6 9.6zM11 6h1v7h-1zm.5 10.5a1 1 0 1 1 1-1 1.002 1.002 0 0 1-1 1z' /></svg>
<mark class='label label-blue margin-right-half'>Calcite Web 2.0 Update</mark>
<p class='leader-1 trailer-0 font-size--1'>
Buttons have received a visual update. Additionally, new opt-in classes have been added, and stateful color class names have been made more consistent. 'btn-grouped' has been removed, please use button group. Our sizing scale has been changed for buttons - sizing ramp has been adjusted. btn-white is now btn-light, a recirprocal btn-dark has been added.
</p>
<p class='leader-half trailer-0 font-size--1'>
New <em>btn-rounded</em>,, <em>btn-red-fill</em>, <em>btn-red-fill</em>, <em>btn-transparent-white</em> have been added. You can combine any sizing modifiers with any coloring modifiers.
</p>

Button green has been removed, we recommend using primary 'btn' class for all leading actions. We've added some red actions to provide options for invoking destructive actions
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

The `btn-link` class also allows you to style inline anchors you wish to receive an underline animation. Here's <a class="btn-link font-size--4">an example of a btn-link</a> within a block of text that may wrap. Sometimes, the proper semantic element is a button, but you would rather the element look more like a link. In these instances, Calcite Web provides an alternate class <a class="btn-link">of a btn-link</a> which styles a button element as if it were a simple anchor:

```html
<button class="btn-link">This is a button</button>
Here's <a class="btn-link">an example of a btn-link</a> within a block of text that may wrap.
```
