# Button

<box header>

    A button component in Vue is a reusable user interface element that represents an interactive element that users can click or tap to trigger an action or perform a specific task. Buttons are one of the fundamental elements in user interfaces and are used for various purposes, such as submitting forms, navigating between pages, triggering events, or executing specific functions.
</box>

<box>

## Default

We have the `v-btn` component.

<vuecode md>
<div slot="demo">
<v-btn>
  Button
</v-btn>

</div>
</vuecode>
</box>

## Props
    A wide array of props can be employed to modify the v-btn component’s look and functionality. Props like prepend-icon and append-icon offer a straightforward approach to incorporate positioned icons, whereas block and stacked props are utilized to manage the component’s form.

### Density
    The density prop is used to control the vertical space that the button takes up.

### Size
    The size property is used to control the size of the button and scales with density. The default size is undefined which essentially translates to medium.

### Block
    Block buttons extend the full available width of their container. This is useful for creating buttons that span the full width of a card or dialog.

### Rounded
    Use the rounded prop to control the border radius of a button.

### Elevation
    The elevation property provides up to 24 levels of shadow depth. By default, buttons rest at 2dp.

### Variants
    The variant prop gives you easy access to several different button styles. Available variants are: elevated(default), flat, tonal, outlined, text, and plain.