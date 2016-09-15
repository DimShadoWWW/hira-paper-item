
<!---

This README is automatically generated from the comments in these files:
paper-icon-item.html  hira-paper-item-behavior.html  hira-paper-item-body.html  hira-paper-item.html

Edit those files, and our readme bot will duplicate them over here!
Edit this file, and the bot will squash your changes :)

The bot does some handling of markdown. Please file a bug if it does the wrong
thing! https://github.com/PolymerLabs/tedium/issues

-->

[![Build status](https://travis-ci.org/PolymerElements/hira-paper-item.svg?branch=master)](https://travis-ci.org/PolymerElements/hira-paper-item)

_[Demo and API docs](https://elements.polymer-project.org/elements/hira-paper-item)_


##&lt;hira-paper-item&gt;

Material design: [Lists](https://www.google.com/design/spec/components/lists.html)

`<hira-paper-item>` is an interactive list item. By default, it is a horizontal flexbox.

```html
<hira-paper-item>Item</hira-paper-item>
```

Use this element with `<hira-paper-item-body>` to make Material Design styled two-line and three-line
items.

```html
<hira-paper-item>
  <hira-paper-item-body two-line>
    <div>Show your status</div>
    <div secondary>Your status is visible to everyone</div>
  </hira-paper-item-body>
  <iron-icon icon="warning"></iron-icon>
</hira-paper-item>
```

To use `hira-paper-item` as a link, wrap it in an anchor tag. Since `hira-paper-item` will
already receive focus, you may want to prevent the anchor tag from receiving
focus as well by setting its tabindex to -1.

```html
<a href="https://www.polymer-project.org/" tabindex="-1">
  <hira-paper-item raised>Polymer Project</hira-paper-item>
</a>
```

If you are concerned about performance and want to use `hira-paper-item` in a `paper-listbox`
with many items, you can just use a native `button` with the `hira-paper-item` class
applied (provided you have correctly included the shared styles):

```html
<style is="custom-style" include="hira-paper-item-shared-styles"></style>

<paper-listbox>
  <button class="hira-paper-item" role="option">Inbox</button>
  <button class="hira-paper-item" role="option">Starred</button>
  <button class="hira-paper-item" role="option">Sent mail</button>
</paper-listbox>
```

### Styling

The following custom properties and mixins are available for styling:

| Custom property | Description | Default |
| --- | --- | --- |
| `--paper-item-min-height` | Minimum height of the item | `48px` |
| `--paper-item` | Mixin applied to the item | `{}` |
| `--paper-item-selected-weight` | The font weight of a selected item | `bold` |
| `--paper-item-selected` | Mixin applied to selected hira-paper-items | `{}` |
| `--paper-item-disabled-color` | The color for disabled hira-paper-items | `--disabled-text-color` |
| `--paper-item-disabled` | Mixin applied to disabled hira-paper-items | `{}` |
| `--paper-item-focused` | Mixin applied to focused hira-paper-items | `{}` |
| `--paper-item-focused-before` | Mixin applied to :before focused hira-paper-items | `{}` |

### Accessibility

This element has `role="listitem"` by default. Depending on usage, it may be more appropriate to set
`role="menuitem"`, `role="menuitemcheckbox"` or `role="menuitemradio"`.

```html
<hira-paper-item role="menuitemcheckbox">
  <hira-paper-item-body>
    Show your status
  </hira-paper-item-body>
  <paper-checkbox></paper-checkbox>
</hira-paper-item>
```



##&lt;hira-paper-icon-item&gt;

`<hira-paper-icon-item>` is a convenience element to make an item with icon. It is an interactive list
item with a fixed-width icon area, according to Material Design. This is useful if the icons are of
varying widths, but you want the item bodies to line up. Use this like a `<hira-paper-item>`. The child
node with the attribute `item-icon` is placed in the icon area.

```html
<hira-paper-icon-item>
  <iron-icon icon="favorite" item-icon></iron-icon>
  Favorite
</hira-paper-icon-item>
<hira-paper-icon-item>
  <div class="avatar" item-icon></div>
  Avatar
</hira-paper-icon-item>
```

### Styling

The following custom properties and mixins are available for styling:

| Custom property | Description | Default |
| --- | --- | --- |
| `--paper-item-icon-width` | Width of the icon area | `56px` |
| `--paper-item-icon` | Mixin applied to the icon area | `{}` |
| `--paper-icon-item` | Mixin applied to the item | `{}` |
| `--paper-item-selected-weight` | The font weight of a selected item | `bold` |
| `--paper-item-selected` | Mixin applied to selected hira-paper-items | `{}` |
| `--paper-item-disabled-color` | The color for disabled hira-paper-items | `--disabled-text-color` |
| `--paper-item-disabled` | Mixin applied to disabled hira-paper-items | `{}` |
| `--paper-item-focused` | Mixin applied to focused hira-paper-items | `{}` |
| `--paper-item-focused-before` | Mixin applied to :before focused hira-paper-items | `{}` |



##&lt;hira-paper-item-body&gt;

Use `<hira-paper-item-body>` in a `<hira-paper-item>` or `<hira-paper-icon-item>` to make two- or
three- line items. It is a flex item that is a vertical flexbox.

```html
<hira-paper-item>
  <hira-paper-item-body two-line>
    <div>Show your status</div>
    <div secondary>Your status is visible to everyone</div>
  </hira-paper-item-body>
</hira-paper-item>
```

The child elements with the `secondary` attribute is given secondary text styling.

### Styling

The following custom properties and mixins are available for styling:

| Custom property | Description | Default |
| --- | --- | --- |
| `--paper-item-body-two-line-min-height` | Minimum height of a two-line item | `72px` |
| `--paper-item-body-three-line-min-height` | Minimum height of a three-line item | `88px` |
| `--paper-item-body-secondary-color` | Foreground color for the `secondary` area | `--secondary-text-color` |
| `--paper-item-body-secondary` | Mixin applied to the `secondary` area | `{}` |



<!-- No docs for Polymer.PaperItemBehavior found. -->
