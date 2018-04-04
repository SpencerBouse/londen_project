<template>
  <div class='container-fluid'>
<<<<<<< HEAD
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
=======
      <navigation></navigation>
      <cover class='col-md-12 animated fadeIn'></cover>
      <aboutContent></aboutContent>
      <musicContent></musicContent>
      <galleryContent></galleryContent>
      <liveContent></liveContent>
      <myfooter></myfooter>
>>>>>>> c5ca2fd7793e943126a5becfc9da78e934dd8f7c
  </div>
</template>

<script>
import Cover from './Cover.vue'
import Navigation from './Navigation.vue'
import MyFooter from './MyFooter.vue'
import AboutContent from './AboutContent.vue'
import MusicContent from './MusicContent.vue'
import GalleryContent from './GalleryContent.vue'
import LiveContent from './LiveContent.vue'

export default {
  name: 'Home',
  components: {
    'cover': Cover,
    'navigation': Navigation,
    'aboutContent': AboutContent,
    'musicContent': MusicContent,
    'galleryContent': GalleryContent,
    'liveContent': LiveContent,
    'myfooter': MyFooter
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang='scss'>
  @import '../../src/assets/sass/now-ui-kit.scss';
</style>
