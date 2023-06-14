# List

<box header>

  Lists are continuous, vertical indexes of text or imagesA list component in Vue is a reusable user interface element that facilitates the display of a collection of items in a structured and organized manner. It is commonly used to present data such as a list of products, messages, contacts, or any other set of related information.
  
  The list component typically consists of a container that holds individual list items. Each list item may contain various elements, such as text, images, icons, buttons, or additional components, to represent the data in a meaningful way.
  
</box>

<box>

## Basic

A basic list of items with `title` and `subtitle`.

<vuecode md>
<div slot="demo">
  <v-list>
    <v-list-item title="One text"></v-list-item>
    <v-list-item title="Another text" subtitle="A little text"></v-list-item>
    <v-list-item title="Some more text"></v-list-item>
    <v-list-item title="Even more text" subtitle="Another little text"></v-list-item>
  </v-list>
</div>
<div slot="code">

```html
  <v-list>
    <v-list-item title="One text"></v-list-item>
    <v-list-item title="Another text" subtitle="A little text"></v-list-item>
    <v-list-item title="Some more text"></v-list-item>
    <v-list-item title="Even more text" subtitle="Another little text"></v-list-item>
  </v-list>
```

</div>
</vuecode>
</box>

<box>

## Header

A `v-list-header` separator with custom `color`.

<vuecode md>
<div slot="demo">
  <v-list>
    <v-list-header title="Group 1"></v-list-header>
    <v-list-item title="Snickerdoodle" subtitle="An excellent companion"></v-list-item>
    <v-list-item title="Sapporo Haru" subtitle="An excellent polish restaurant, quick delivery and hearty, filling meals"></v-list-item>
    <v-list-header title="Group 2" color="success"></v-list-header>
    <v-list-item title="Enid's" subtitle="At night a bar, during the day a delicious brunch spot."></v-list-item>
    <v-list-item title="Veronika Ossi" subtitle="Has not watched anything recently"></v-list-item>
  </v-list>
</div>
<div slot="code">

```html
  <v-list>
    <v-list-header title="Group 1"></v-list-header>
    <v-list-item title="Snickerdoodle" subtitle="An excellent companion"></v-list-item>
    <v-list-item title="Sapporo Haru" subtitle="An excellent polish restaurant, quick delivery and hearty, filling meals"></v-list-item>
    <v-list-header title="Group 2" color="success"></v-list-header>
    <v-list-item title="Enid's" subtitle="At night a bar, during the day a delicious brunch spot."></v-list-item>
    <v-list-item title="Veronika Ossi" subtitle="Has not watched anything recently"></v-list-item>
  </v-list>
```

</div>
</vuecode>
</box>

<box>

## Content

You can add custom content to the item. It will be pushed to the right side.

<vuecode md>
<div slot="demo">
  <v-list>
    <v-list-header title="Group 1"></v-list-header>
    <v-list-item title="Rachel" subtitle="Last seen watching Arrested Development just now.">
      <v-button color="danger">One action</v-button>
    </v-list-item>
    <v-list-item title="Lindsay" subtitle="Last seen watching Bob's Burgers 10 hours ago.">
      <v-checkbox color="danger"/>
    </v-list-item>
    <v-list-header title="Group 2" color="success"></v-list-header>
    <v-list-item title="Enid's" subtitle="At night a bar, during the day a delicious brunch spot.">
      <v-chip color="warning">Another component</v-chip>
    </v-list-item>
    <v-list-item title="Veronika Ossi" subtitle="Has not watched anything recently">
      <v-switch color="warning"/>
    </v-list-item>
  </v-list>
</div>
<div slot="code">

```html
  <v-list>
    <v-list-header title="Group 1"></v-list-header>
    <v-list-item title="Snickerdoodle" subtitle="An excellent companion">
      <v-button color="danger">One action</v-button>
    </v-list-item>
    <v-list-item title="Sapporo Haru" subtitle="An excellent polish restaurant, quick delivery and hearty, filling meals">
      <v-checkbox color="danger"/>
    </v-list-item>
    <v-list-header title="Group 2" color="success"></v-list-header>
    <v-list-item title="Enid's" subtitle="At night a bar, during the day a delicious brunch spot.">
      <v-chip color="warning">Another component</v-chip>
    </v-list-item>
    <v-list-item title="Veronika Ossi" subtitle="Has not watched anything recently">
      <v-switch color="warning"/>
    </v-list-item>
  </v-list>
```

</div>
</vuecode>
</box>

<box>
