<template id="modal-template">
  <div class="modal-backdrop">
    <div class="modal">
      <div @click='closeModal()'>X</div>
      <img :src='imageSrc'/>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Modal',
  methods: {
    closeModal () {
      Event.$emit('closeModal')
    }
  },
  data () {
    return {
      imageSrc: this.$attrs.imageSrc
    }
  }
}
</script>

<style lang='scss'>
  @import '../../src/assets/sass/now-ui-kit.scss';
</style>
