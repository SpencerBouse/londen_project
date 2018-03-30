<template>
  <div class='mainContent'>
    <aboutContent v-if='tabs.showAbout'></aboutContent>
    <musicContent v-if='tabs.showMusic'></musicContent>
    <galleryContent v-if='tabs.showGallery'></galleryContent>
    <liveContent v-if='tabs.showLive'></liveContent>
  </div>
</template>

<script>
// import Vue from 'vue'
import AboutContent from './AboutContent.vue'
import MusicContent from './MusicContent.vue'
import GalleryContent from './GalleryContent.vue'
import LiveContent from './LiveContent.vue'

export default {
  name: 'MainContent',
  components: {
    'aboutContent': AboutContent,
    'musicContent': MusicContent,
    'galleryContent': GalleryContent,
    'liveContent': LiveContent
  },
  data () {
    return {
      tabs: {
        showAbout: true,
        showMusic: false,
        showGallery: false,
        showLive: false
      }
    }
  },
  created () {
    var q = this.$route.query
    var tabs = this.tabs
    let self = this

    Event.$on('setQuery', function (t) {
      change(t)
    })

    function change (value) {
      value = 'show' + value
      Object.keys(tabs).forEach(function (key) {
        self.$set(tabs, key, false)
      })
      Object.keys(tabs).forEach(function (key) {
        if (key === value) {
          self.$set(tabs, key, true)
        }
      })
    }

    if (q.tags) {
      change(q.tags)
    } else {
      this.$router.push({path: '/', query: { tags: 'about' }})
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang='scss'>
  @import '../../src/assets/sass/now-ui-kit.scss';
</style>
