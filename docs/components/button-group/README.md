# Button group

> Group a series of buttons together on a single line with `<b-button group>`.

**Example 1:** Default, Small, and Large button groups
```html
<div>
  <b-button-group>
    <b-button>Button 1</b-button>
    <b-button>Button 2</b-button>
    <b-button>Button 3</b-button>
  </b-button-group>
  <br>
  <br>
  <b-button-group size="sm">
    <b-button>Left</b-button>
    <b-button>Middle</b-button>
    <b-button>Right</b-button>
  </b-button-group>
  <br>
  <br>
  <b-button-group size="lg">
    <b-button>Left</b-button>
    <b-button>Middle</b-button>
    <b-button>Right</b-button>
  </b-button-group>
</div>

<!-- button-group-1.vue -->
```

**Example 2:** Default button group with contextual variants
```html
<div>
  <b-button-group>
    <b-button variant="success">Success</b-button>
    <b-button variant="info">Info</b-button>
    <b-button variant="warning">Warning</b-button>
    <b-button variant="primary">Primary</b-button>
    <b-button variant="danger">Danger</b-button>
    <b-button variant="link">Link</b-button>
  </b-button-group>
</div>

<!-- button-group-2.vue -->
```

**Example 3:** button group with dropdown menus
```html
<div>
  <b-button-group>
    <b-button>Button 1</b-button>
    <b-button>Button 2</b-button>
    <b-dropdown right text="Menu">
      <b-dropdown-item>Item 1</b-dropdown-item>
      <b-dropdown-item>Item 2</b-dropdown-item>
      <b-dropdown-divider></b-dropdown-divider>
      <b-dropdown-item>Item 3</b-dropdown-item>
    </b-dropdown>
    <b-button>Button 3</b-button>
    <b-dropdown right split text="Split Menu">
      <b-dropdown-item>Item 1</b-dropdown-item>
      <b-dropdown-item>Item 2</b-dropdown-item>
      <b-dropdown-divider></b-dropdown-divider>
      <b-dropdown-item>Item 3</b-dropdown-item>
    </b-dropdown>
  </b-button-group>
</div>

<!-- button-group-3.vue -->
```

**Example 4:** Vertical button group
```html
<div>
  <b-button-group vertical>
    <b-button>Top</b-button>
    <b-button>Middle</b-button>
    <b-button>Bottom</b-button>
  </b-button-group>
</div>

<!-- button-group-4.vue -->
```

### Sizing
Set the size prop to `lg` or `sm` to render larger or smaller, respectively, buttons.
There is no need to specify the size on the individual buttons.

### Vertical variation
Make a set of buttons appear vertically stacked rather than horizontally by setting
the `vertical` prop. Split button dropdowns are not supported here.

### Dropdown menu support
Add [`<b-dropdown>`](./dropdown) menus directly inside your `<b-button-group>`. Note
that split dropdown menus are not supported when prop `vertical` is set.

### Alias
`<b-button-group>` can also be used by its shorter alias `<b-btn-group>`.

### See also
Also check out the [`<b-button-toolabr>`](./button-toolbar) component for generating
toolbars containing button groups and input groups.

### Tooltips and popovers
Due to the specific implementation (and some other components), tooltips and popovers
on elements within a button-group will have adverse effect on styling.
