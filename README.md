# Decor CSS

_Decor_ makes your default HTML look nicer.

It is easy to customize or cherry-pick.

No pre/post-compiler, just plain basic CSS.

[Demo page](https://polight.github.io/decor)


## Usage

Add the CSS to your HTML to get your site <em>decor</em>ated.

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/polight/decor@master/decor.css">
```

Your default HTML will be beautifully repainted.

## Advanced Usage

You may restrict usage of Decor to only some type of component, or want to customize.

To do so, import only the _parts_ you want, eventually in a main css file of your own:

```CSS
@import url('https://cdn.jsdelivr.net/gh/polight/decor@master/parts/reset.css');
@import url('https://cdn.jsdelivr.net/gh/polight/decor@master/parts/vars.css');
@import url('/css/my-custom-vars.css');
@import url('https://cdn.jsdelivr.net/gh/polight/decor@master/parts/tags.css');
@import url('https://cdn.jsdelivr.net/gh/polight/decor@master/parts/buttons.css');
@import url('https://cdn.jsdelivr.net/gh/polight/decor@master/parts/grids.css');
@import url('https://cdn.jsdelivr.net/gh/polight/decor@master/parts/forms.css');
@import url('https://cdn.jsdelivr.net/gh/polight/decor@master/parts/toolbars.css');
```

> This is a quick sample. You probably want to download Decor with a specific version to stabilize the behavior.

## Advanced Styles

To provide with a more advanced styling, Decor provides you with some basic classes:

### Grid

- `class="row"`: aligns children on the same line. Conveninent to get 2 elements besides each others.
- `class="row spaced"`: aligned items with maximum space between each other.
- `class="secondary"`: should be used on a child of a `class="row"` and will align the element to the right.

### Buttons

Buttons are styled by default.
Some classes give a specific style:
- `<button class="primary">`: the button is a main action.
- `<button class="plain">`: the button behaves similarly to a link.
- `<button class="danger">`: the button is a dangerous action, like an error a deletion.
- `<button class="primary danger">`: the button is a primary dangerous action.
- `<a class="button">` will make a link look like a button. Same _primary_, _plain_ and _danger_ classes may be added.

### Toolbar Widget

- `class="toolbar"`: provides a sticky toolbar. Great to have an action toolbar at the bottom of a section.
