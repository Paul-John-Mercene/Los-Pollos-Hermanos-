# Progress

<box header>
    A progress component in Vue is a user interface element that visually represents the progress or completion of a task, process, or operation. It is commonly used to provide feedback to users about the status of an ongoing action, such as file uploads, form submissions, or loading processes.
    
    The progress component typically consists of a horizontal bar or a circular indicator that fills up or advances based on the completion percentage. 

</box>


<box>

## Colors

Nice colors for your progress bar.

<vuecode md>
<div slot="demo">
  <v-progress :percent="100" color="primary">primary</v-progress>
  <v-progress :percent="90" color="warning">warning</v-progress>
  <v-progress :percent="75" color="danger">danger</v-progress>
  <vs-progress :percent="60" color="success">success</v-progress>
  <v-progress :percent="45" color="dark">dark</v-progress>
  <v-progress :percent="30" color="rgb(164, 69, 15)">RGB</v-progress>
  <v-progress :percent="15" color="#24c1a0">HEX</v-progress>
</div>
<div slot="code">

```html
  <v-progress :percent="100" color="primary">primary</v-progress>
  <v-progress :percent="90" color="warning">warning</v-progress>
  <v-progress :percent="75" color="danger">danger</v-progress>
  <v-progress :percent="60" color="success">success</v-progress>
  <vs-progress :percent="45" color="dark">dark</vs-progress>
  <v-progress :percent="30" color="rgb(164, 69, 15)">RGB</v-progress>
  <v-progress :percent="15" color="#24c1a0">HEX</v-progress>
```

</div>
</vuecode>

</box>


<box>

## Indeterminate

You can have a progress bar with indeterminate value with the property `indeterminate`.

<vuecode md>
<div slot="demo">
  <v-progress indeterminate color="primary">primary</v-progress>
</div>
<div slot="code">

```html
  <v-progress indeterminate color="primary">primary</v-progress>
```

</div>
</vuecode>

</box>


<box>

## Height

You can change the height of the loading bar with the property `height`.

:::tip
By default the property `height` is **5** (`5px`)
:::

<vuecode md>
<div slot="demo">
  <v-progress :height="2" :percent="100" color="primary">primary</v-progress>
  <v-progress :height="4" :percent="80" color="warning">warning</v-progress>
  <v-progress :height="8" :percent="60" color="danger">danger</v-progress>
  <v-progress :height="12" :percent="40" color="success">success</v-progress>
</div>
<div slot="code">

```html
<v-progress :height="2" :percent="100" color="primary">primary</v-progress>
<v-progress :height="4" :percent="80" color="warning">warning</v-progress>
<v-progress :height="8" :percent="60" color="danger">danger</v-progress>
<v-progress :height="12" :percent="40" color="success">success</v-progress>
```

</div>
</vuecode>

</box>