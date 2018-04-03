<template id="modal-template">
  <div class="modal-backdrop">
    <div class="modal">
      <div @click='closeModal()'><font-awesome-icon :icon="icon" class='modalClose'/> </div>
      <img :src='imageSrc'/>
    </div>
  </div>
</template>

<script>
import FontAwesomeIcon from '@fortawesome/vue-fontawesome'
import faTimes from '@fortawesome/fontawesome-free-solid/faTimes'

export default {
  name: 'Modal',
  computed: {
    icon () {
      return faTimes
    }
  },
  methods: {
    closeModal () {
      Event.$emit('closeModal')
    }
  },
  components: {
    FontAwesomeIcon
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
