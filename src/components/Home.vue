<template>
  <div class='container-fluid'>
    <navigation></navigation>
      <div class='row'>
        <cover class='col-md-12'></cover>
      </div>
      <aboutContent></aboutContent>
      <galleryContent></galleryContent>
      <liveContent></liveContent>
      <!-- <musicContent></musicContent> -->
      <myfooter></myfooter>
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
