<template>
  <div class='gallery-container'>
    <h1>Gallery</h1>
    <img class='col-md-3 galleryPic' src='/static/img/Londen4.jpg' @click="openModal('/static/img/Londen4.jpg')">
    <img class='col-md-3 galleryPic' src='/static/img/Londen3.jpg' @click="openModal('/static/img/Londen3.jpg')">
    <img class='col-md-3 galleryPic' src='/static/img/Londen2.jpg' @click="openModal('/static/img/Londen2.jpg')">
    <img class='col-md-3 galleryPic' src='/static/img/Londen.jpg' @click="openModal('/static/img/Londen.jpg')">
    <img class='col-md-3 galleryPic' src='/static/img/Londen5.jpg' @click="openModal('/static/img/Londen5.jpg')">
    <modal v-if="showModal" @close="showModal = false" :imageSrc='imageSrc' :showModal='showModal'></modal>
  </div>
</template>

<script>
import Modal from './Modal.vue'

export default {
  name: 'GalleryContent',
  methods: {
    openModal (i) {
      this.$set(this.$data, 'imageSrc', i)
      this.$set(this.$data, 'showModal', true)
    }
  },
  components: {
    'modal': Modal
  },
  data () {
    return {
      showModal: false,
      imageSrc: null
    }
  },
  created () {
    let self = this

    Event.$on('closeModal', function () {
      closeModal()
    })

    function closeModal () {
      self.$set(self.$data, 'showModal', false)
    }
  }
}
</script>

<style lang='scss'>
  @import '../../src/assets/sass/now-ui-kit.scss';

  .gallery-container{
    margin-top: 50px
  }
</style>
