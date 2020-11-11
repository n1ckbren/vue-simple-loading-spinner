<script>
import Vue from 'vue';
import { VueSimpleLoadingSpinner } from '@/entry';

export default Vue.extend({
  name: 'ServeDev',
  components: {
    VueSimpleLoadingSpinner,
  }
});
</script>

<template>
  <div id="app">
    <vue-simple-loading-spinner />
  </div>
</template>