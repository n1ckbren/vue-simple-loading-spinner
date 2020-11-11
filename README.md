# vue-simple-loading-spinner

> Collection of loading spinners. No CSS. Command Line Style

## Installation

``` bash
yarn add vue-simple-loading-spinner
```

## Usage

``` vue
<template>
  <div id="app">
    <vue-simple-loading-spinner delay="300" animation="dots" style_class="my_class" />
  </div>
</template>

<script>
  import { VueSimpleLoadingSpinner } from "vue-simple-loading-spinner"
  export default {
    components: {
      VueSimpleLoadingSpinner
    }
  }
</script>
```

## Parameters

``` bash
"delay" (in ms, default: '100')

<vue-simple-loading-spinner delay="300" />
```

``` bash
"animation" (default: 'arrows)

<vue-simple-loading-spinner animation="dots" />
```

``` bash
"style_class" (default: 'vsls-spinner')

<vue-simple-loading-spinner style_class="my_class" />
```

## Animations

``` bash
  ARROWS
  BURGER
  DARK_HEIGHT_PULSE
  DARK_WIDTH_PULSE
  DOTS
  FOUR_DOTS
  MISC_1
  MISC_2
  POINTS_2
  POINTS
  PULSE
  SLASHES
```