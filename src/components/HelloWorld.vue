<template>
  <div class="hello">
    <div class="container">
      <div class="row">
        <div class="col-md-1">
          <p>Hewwo</p>
          <button type="button" name="button" class="btn btn-primary">Test</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang='scss'>
  @import '../../src/assets/css/now-ui-kit.css';
</style>
