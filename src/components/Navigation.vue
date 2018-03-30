<template>
  <div>
    <ul class='nav-bar'>
      <li v-on:click="change('About')">About</li>
      <li v-on:click="change('Music')">Music</li>
      <li v-on:click="change('Gallery')">Gallery</li>
      <li v-on:click="change('Live')">Live</li>
    </ul>
  </div>
</template>

<script>
import Vue from 'vue'

export default {
  name: 'Navigation',
  methods: {
    change: function (t) {
      this.$router.push({path: '/', query: { tags: t }})
      Event.$emit('setQuery', t)
    }
  },
  created () {
    window.Event = new Vue()
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang='scss'>
  @import '../../src/assets/sass/now-ui-kit.scss';
</style>
