<template>
  <span ref="spinner" v-bind:class="this.style_class"></span>
</template>

<script>
import Spinners from './spinners'
export default {
  name: "VueSimpleLoadingSpinner",
  props: {
    delay: {
      type: [Number, String],
      default: 100
    },
    animation: {
      type: String,
      default: "ARROWS"
    },
    style_class: {
      type: String,
      default: "vsls-spinner"
    }
  },

  mounted() {
    this.$nextTick(function () {
      this.spin(this.delay, this.animation);
    });
  },

  methods:{
    spin(delay, animation){
      delay = Number.parseInt(delay);
      animation = animation.toUpperCase();
      let array_to_animate = Spinners[animation];
      let i = 0;
      let self = this;
      setInterval(function() {
        length = array_to_animate.length
          if (i < (array_to_animate.length)) {
            self.$refs.spinner.innerText = array_to_animate[i];
            i++
          } else {
            i = 0
          }
      }, delay)
    }
  }
};
</script>