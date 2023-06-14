# Divider

<box header>

 The divided component in Vue is a reusable user interface element that visually separates content into distinct sections or divisions. It is commonly used to create a clear visual hierarchy within a page or layout by adding visual dividers between different sections or groups of content.
 
 The divided component typically consists of horizontal or vertical lines, borders, or spacing elements that visually separate content. It helps improve readability, organization, and user experience by visually distinguishing different parts of the interface.

</box>

<box>

## Default

You can add a line to divide with the component `v-divider`.

<vuecode md>
<div slot="demo">
 Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
  <v-divider/>
Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
</div>
<div slot="code">

```html
Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
<v-divider/>
Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
```

</div>
</vuecode>
</box>

<box>

## Text

You can add a text between the line to delimit two elements and have a description for the user.

     <vuecode md>
     <div slot="demo">
       Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla    pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
       <v-divider>
         My Text
       </v-divider>
     Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
     </div>
     <div slot="code">

 ```html
 Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
  <v-divider>
    My Text
  </v-divider>
 Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
 ```

 </div>
 </vuecode>
 </box>


 <box>

## Text Position

You can guide the text in **5** ways with property `position`:

- left
- left-center
- center (`default`)
- right-center
- right

<vuecode md>
<div slot="demo">
  <v-divider position="left">
    left
  </v-divider>
  <v-divider position="left-center">
    left-center
  </v-divider>
  <v-divider>
    center (default)
  </v-divider>
  <v-divider position="right-center">
    right-center
  </v-divider>
  <v-divider position="right">
    right
  </v-divider>
</div>
<div slot="code">

```html
<v-divider position="left">
  My Text
</v-divider>
<v-divider position="left-center">
  My Text
</v-divider>
<v-divider position="center">
  My Text
</v-divider>
<v-divider position="right-center">
  My Text
</v-divider>
<v-divider position="right">
  My Text
</v-divider>
```

</div>
</vuecode>
</box>

<box>

## Color

You can change the color of the component with the property `color`, you can use the [main](/theme/) colors or **RGB** and **HEX**.
:::warning
  Only **RGB** and **HEX** colors are supported.
:::

<vuecode md>
<div slot="demo">
  <v-divider>Default</v-divider>
  <v-divider color="primary">Primary</v-divider>
  <v-divider color="success">Success</v-divider>
  <v-divider color="danger">Danger</v-divider>
  <v-divider color="warning">Warning</v-divider>
  <v-divider color="dark">Dark</v-divider>
  <v-divider color="rgb(29, 222, 194)">RGB</v-divider>
  <v-divider color="#ad289f">HEX</v-divider>
</div>
<div slot="code">

```html
<div slot="demo">
  <v-divider>Default</v-divider>
  <v-divider color="primary">Primary</v-divider>
  <v-divider color="success">Success</v-divider>
  <v-divider color="danger">Danger</v-divider>
  <v-divider color="warning">Warning</v-divider>
  <v-divider color="dark">Dark</v-divider>
  <v-divider color="rgb(29, 222, 194)">RGB</v-divider>
  <v-divider color="#ad289f">HEX</v-divider>
</div>
```

</div>
</vuecode>
</box>


<box>

## Background

You can change the background of the text with the property `background`, you can use the [main](/theme/) colors or **RGB** and **HEX**.
:::warning
  Only **RGB** and **HEX** colors are supported.
:::

<vuecode md>
<div slot="demo">
  <v-divider>Default</v-divider>
  <v-divider background="primary" color="#ade6d4">Primary</v-divider>
  <v-divider background="success" color="#0a540a">Success</v-divider>
  <v-divider background="danger" color="lightred">Danger</v-divider>
  <v-divider background="warning" color="grey">Warning</v-divider>
  <v-divider background="dark" color="lightgrey">Dark</v-divider>
  <v-divider background="rgb(252, 243, 192)" color="rgb(29, 222, 194)">RGB</v-divider>
  <v-divider background="#fffaaa" color="#ad289f">HEX</v-divider>
</div>
<div slot="code">

```html
<div slot="demo">
  <v-divider>Default</v-divider>
  <v-divider background="primary" color="#ade6d4">Primary</v-divider>
  <v-divider background="success" color="#0a540a">Success</v-divider>
  <v-divider background="danger" color="lightred">Danger</v-divider>
  <v-divider background="warning" color="grey">Warning</v-divider>
  <v-divider background="dark" color="lightgrey">Dark</v-divider>
  <v-divider background="rgb(252, 243, 192)" color="rgb(29, 222, 194)">RGB</v-divider>
  <v-divider background="#fffaaa" color="#ad289f">HEX</v-divider>
</div>
```

</div>
</vuecode>
</box>


<box>
