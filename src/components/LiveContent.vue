<template>
  <div class='live-container'>
    <h1>Live</h1>
    <iframe class='tickets' src="//ticketbud.com/events/439e4a70-f174-11e7-a239-3f71614bba7b/external"></iframe>
  </div>
</template>

<script>
export default {
  name: 'LiveContent'
}
</script>

<style lang='scss'>
  @import '../../src/assets/sass/now-ui-kit.scss';

  .tickets{
    background-color: white;
    width: 90%;
    height: 26em;
  }

  .live-container{
    background: linear-gradient($purple-bg, $darkpurple-bg);
    padding-top: 100px;
  }
</style>
