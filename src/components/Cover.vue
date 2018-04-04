<template>
  <div class='fullCover'>
      <div class='row'>
        <img class="cover" src='/static/img/Londen4.jpg'>
      </div>
  </div>
</template>

<script>
import MainContent from './MainContent.vue'

export default {
  name: 'Cover',
  components: {
    'mainContent': MainContent
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang='scss'>
  @import '../../src/assets/sass/now-ui-kit.scss';

  .fullCover{
    background: linear-gradient($purple-bg, $darkpurple-bg);
    div{
      float: right;
    }
    .cover {
      height: 30em;
    }
    @media (min-width: $screen-sm-min) {

    }
    @media (min-width: $screen-md-min) {
      .cover{
        height: 100vh;
        float: right;
      }
    }
    @media (min-width: $screen-lg-min) {

    }
  }

</style>
