# Card

<box header>

  A card component in Vue is a reusable user interface element that represents a container for displaying related content. It is commonly used to present organized information or data in a visually appealing and structured manner.
  
  The card component typically consists of a rectangular container with a distinct style, which may include elements such as a header, body, footer, and optional image or icon. It provides a flexible structure that allows developers to customize the content and appearance based on their specific requirements.
</box>

<box>

## Default

To add a card we have the `v-card` component, for the internal structure we use several **slots** (`header`, `footer`, `media`, ... )

<vuecode md>
<div slot="demo">
<vs-row vs-justify="center">
  <vs-col type="flex" vs-justify="center" vs-align="center" vs-w="6">
    <vs-card>
      <div slot="header">
        <h3>
          Hello world !
        </h3>
      </div>
      <div>
        <span>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</span>
      </div>
      <div slot="footer">
        <vs-row vs-justify="flex-end">
          <vs-button type="gradient" color="danger" icon="favorite"></vs-button>
          <vs-button color="primary" icon="turned_in_not"></vs-button>
          <vs-button color="rgb(230,230,230)" color-text="rgb(50,50,50)" icon="settings"></vs-button>
        </vs-row>
      </div>
    </v-card>
  </vs-col>
</vs-row>
</div>
<div slot="code">

```html
<vs-row vs-justify="center">
  <vs-col type="flex" vs-justify="center" vs-align="center" vs-w="6">
    <vs-card>
      <div slot="header">
        <h3>
          Hello world !
        </h3>
      </div>
      <div>
        <span>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</span>
      </div>
      <div slot="footer">
        <vs-row vs-justify="flex-end">
          <vs-button type="gradient" color="danger" icon="favorite"></vs-button>
          <vs-button color="primary" icon="turned_in_not"></vs-button>
          <vs-button color="rgb(230,230,230)" color-text="rgb(50,50,50)" icon="settings"></vs-button>
        </vs-row>
      </div>
    </vs-card>
  </vs-col>
</vs-row>
```

</div>
</vuecode>
</box>

<box>

## Media

There are cases in which you need to add an image or video on the card so we have the `slot="media"`

<vuecode md>
<div slot="demo">
  <Demos-Card-Media />
</div>
<div slot="code">

```html
<template>
  <vs-row vs-justify="center">
    <vs-col type="flex" vs-justify="center" vs-align="center" vs-w="6">
      <v-card class="cardx">
        <div slot="header">
          <h3>
            Hello world !
          </h3>
        </div>
        <div slot="media">
          <img :src="$withBase('/card.png')">
        </div>
        <div>
          <span>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</span>
        </div>
        <div slot="footer">
          <vs-row vs-justify="flex-end">
            <vs-button type="gradient" color="danger" icon="favorite"></vs-button>
            <vs-button color="primary" icon="turned_in_not"></vs-button>
            <vs-button color="rgb(230,230,230)" color-text="rgb(50,50,50)" icon="settings"></vs-button>
          </vs-row>
        </div>
      </v-card>
    </vs-col>
    <vs-col type="flex" vs-justify="center" vs-align="center" vs-w="6">
      <v-card class="cardx">
        <div slot="header">
          <h3>
            Hello world !
          </h3>
        </div>
        <div slot="media">
          <img :src="$withBase('/card2.png')">
        </div>
        <div>
          <span>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</span>
        </div>
        <div slot="footer">
          <vs-row vs-justify="flex-end">
            <vs-button type="gradient" color="danger" icon="favorite"></vs-button>
            <vs-button color="primary" icon="turned_in_not"></vs-button>
            <vs-button color="rgb(230,230,230)" color-text="rgb(50,50,50)" icon="settings"></vs-button>
          </vs-row>
        </div>
      </v-card>
    </vs-col>
  </vs-row>
</template>
<script>
export default {

}
</script>
<style lang="stylus">
.cardx
  margin 15px
</style>
```

</div>
</vuecode>
</box>

<box>

## Fixed Height

If you need to set card with the same height, send the prop `fixed-height` and cards set to 100% of height.

<vuecode md>
<div slot="demo">
  <Demos-Card-FixedHeight />
</div>
<div slot="code">

```html
<template>
  <vs-row vs-justify="center">
    <vs-col type="flex" vs-justify="center" vs-align="center" vs-w="6">
      <v-card class="cardx" fixedHeight>
        <div slot="header">
          <h3>
            Hello world !
          </h3>
        </div>
        <div slot="media">
          <img :src="$withBase('/card.png')">
        </div>
        <div>
          <span>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</span>
          <span>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</span>
        </div>
        <div slot="footer">
          <vs-row vs-justify="flex-end">
            <vs-button type="gradient" color="danger" icon="favorite"></vs-button>
            <vs-button color="primary" icon="turned_in_not"></vs-button>
            <vs-button color="rgb(230,230,230)" color-text="rgb(50,50,50)" icon="settings"></vs-button>
          </vs-row>
        </div>
      </vs-card>
    </vs-col>
    <vs-col type="flex" vs-justify="center" vs-align="center" vs-w="6">
      <v-card class="cardx" fixedHeight>
        <div slot="header">
          <h3>
            Hello world !
          </h3>
        </div>
        <div slot="media">
          <img :src="$withBase('/card2.png')">
        </div>
        <div>
          <span>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</span>
        </div>
        <div slot="footer">
          <vs-row vs-justify="flex-end">
            <vs-button type="gradient" color="danger" icon="favorite"></vs-button>
            <vs-button color="primary" icon="turned_in_not"></vs-button>
            <vs-button color="rgb(230,230,230)" color-text="rgb(50,50,50)" icon="settings"></vs-button>
          </vs-row>
        </div>
      </v-card>
    </vs-col>
  </vs-row>
</template>
<script>
export default {

}
</script>
<style lang="stylus">
.cardx
  margin 15px
</style>

```

</div>
</vuecode>
</box>

<box>