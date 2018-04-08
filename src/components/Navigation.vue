<template>
  <div>
    <ul class='nav-bar'>
      <li class='underline' v-on:click="change('About')">About</li>
      <li class='underline' v-on:click="change('Music')">Music</li>
      <li class='underline' v-on:click="change('Gallery')">Gallery</li>
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

  .nav-bar{
    position: absolute;
    left: 0px;
    font-size: 1.5em;
    padding: 15px;
    z-index: 999;
    li{
      text-align: center;
      cursor: pointer;
      display: inline;
      padding-right: 10px;
    }
  }
</style>
