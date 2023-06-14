# Textarea
<box header>

 A textarea component in Vue is a user interface element that enables users to input and edit multi-line text. It provides a resizable text input field that allows users to enter longer blocks of text, such as paragraphs or comments. The textarea component can be easily customized and integrated into Vue applications, offering features like value binding, placeholder text, rows and columns configuration, disabled and read-only modes, event handling, and more.

</box>

<box>

## Default

To add a **Textarea** we have the component `vs-textarea`

<vuecode md>
<div slot="demo">
  <Demos-Textarea-Default />
</div>
<div slot="code">

```html
<template lang="html">
  <div>
    <vs-textarea v-model="textarea" />
  </div>
</template>

<script>
export default {
  data:()=>({
    textarea: '',
  })
}
</script>
```

</div>
</vuecode>
</box>

<box>

## Label

If you need to add a label you can use the `label` property

<vuecode md>
<div slot="demo">
  <Demos-Textarea-Label />
</div>
<div slot="code">

```html
<template lang="html">
  <div>
    <vs-textarea label="Label in Textarea" v-model="textarea" />
  </div>
</template>

<script>
export default {
  data:()=>({
    textarea: '',
  })
}
</script>
```

</div>
</vuecode>
</box>

<box>

## Width

You can set the width of the textarea width the `width` property. You can also use css values like`10rem` or `50%` as value.

<vuecode md>
<div slot="demo">
  <Demos-Textarea-Width />
</div>
<div slot="code">

```html
<template lang="html">
  <div>
    <vs-textarea label="Width set to 300px" width="300px" />
  </div>
</template>
```

</div>
</vuecode>
</box>

<box>

## Height

You can set the height of the textarea with the `height` property. You can also use css values like`10rem` or `50%` as value.

<vuecode md>
<div slot="demo">
  <Demos-Textarea-Height />
</div>
<div slot="code">

```html
<template lang="html">
  <div>
    <vs-textarea label="Height set to 200px" height="200px" />
  </div>
</template>
```

</div>
</vuecode>
</box>