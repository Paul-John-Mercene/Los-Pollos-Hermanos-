# Images

<box header>

An images component in Vue is a reusable user interface element that allows developers to display and manipulate images within their Vue applications. It provides a way to easily handle and render images, whether they are local files or fetched from external sources.

The images component typically accepts image URLs or file paths as input and renders the corresponding images on the web page. 

</box>

<box>

## Default

You can create an image gallery easily with the components `v-img`

<vuecode md>
<div slot="demo">
  <Demos-Images-Default />
</div>
<div slot="code">

```html
<template lang="html">
  <div class="con-example-images">
    <v-img>
      <v-img :key="index" :src="`https://picsum.photos/400/400?image=2${index}`" v-for="(image, index) in 9" />
      <v-img :key="index" :src="`https://picsum.photos/400/400?image=1${index}`" v-for="(image, index) in 7" />
    </v-img>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="stylus">
.con-example-images
  max-height 500px
  overflow auto
</style>
```

</div>
</vuecode>
</box>

<box>

## Other Information

You can make changes in some details like removing the border-radius with the property `not-border-radius` or adding a different style of layout with the property `alternating`, you can also remove the margin between the images with the property `not- margin`.

<vuecode md>
<div slot="demo">
  <Demos-Images-More />
</div>
<div slot="code">

```html
<template lang="html">
  <div class="con-example-images">
    <v-img alternating not-border-radius not-margin >
      <v-img :key="index" :src="`https://picsum.photos/400/400?image=3${index}`" v-for="(image, index) in 9" />
      <v-img :key="index" :src="`https://picsum.photos/400/400?image=4${index}`" v-for="(image, index) in 7" />
    </v-img>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="stylus">
.con-example-images
  max-height 500px
  overflow auto
</style>
```

</div>
</vuecode>
</box>
