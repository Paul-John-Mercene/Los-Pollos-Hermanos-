# Toolbar

<box header>

    A toolbar component in Vue is a reusable user interface element that provides a collection of buttons, icons, and other interactive elements for quick access to frequently used actions or functionality within an application. It is commonly used to create a navigation or action bar at the top or bottom of a page or screen.
    
    The toolbar component typically consists of a horizontal or vertical container that holds various interactive elements, such as buttons, icons, dropdowns, or input fields
</box>

<box>

## Default

We have the `v-toolbar` component. The toolbar component works great in conjunction with `v-navigation-drawer`and `v-card`. 

    <vuecode md>
    <div slot="demo">
    <v-toolbar title="Application"></v-toolbar>
    </div>
    </vuecode>
    </box>

## Props
    A wide array of props can be employed to modify the v-toolbar component’s look and functionality.

### Background
    Toolbars can display a background as opposed to a solid color using the src prop. This can be modified further by using the img slot and providing your own v-img component. Backgrounds can be faded using a v-app-bar.

### Collapse
    Toolbars can be collapsed to save screen space.

### Dense toolbars
    Dense toolbars reduce their height to 48px. When using in conjunction with the prominent prop, will reduce height to 96px.

### Extended
    Toolbars can be extended without using the extension slot.

### Floating with search
    A floating toolbar is turned into an inline element that only takes up as much space as needed. This is particularly useful when placing toolbars over content.

### Variations
    A v-toolbar has multiple variations that can be applied with themes and helper classes. These range from light and dark themes, colored and transparent.
