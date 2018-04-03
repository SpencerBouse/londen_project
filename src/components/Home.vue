<template>
  <div class='container-fluid'>
    <navigation></navigation>
      <div class='row'>
        <cover class='col-md-12'></cover>
      </div>
      <div class='row'>
        <mainContent class='col-md-12'></mainContent>
      </div>
      <div class='row'>
        <myfooter class='col-md-6 offset-md-3'></myfooter>
    </div>
  </div>
</template>

<script>
import Cover from './Cover.vue'
import Navigation from './Navigation.vue'
import MainContent from './MainContent.vue'
import MyFooter from './MyFooter.vue'

export default {
  name: 'Home',
  components: {
    'cover': Cover,
    'navigation': Navigation,
    'mainContent': MainContent,
    'myfooter': MyFooter
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang='scss'>
  @import '../../src/assets/sass/now-ui-kit.scss';
</style>
