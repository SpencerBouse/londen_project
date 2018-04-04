<template>
  <div>
    <ul class='iconContainer row'>
      <li class='icon col-md-2'>
        <a href='https://www.facebook.com/ChrisLonden3AM/'>
          <font-awesome-icon :icon="facebook"/>
          <p>Facebook</p>
        </a>
      </li>
      <li class='icon col-md-2'>
        <a href='https://www.instagram.com/chrislondenmusic/'>
          <font-awesome-icon :icon="instagram"/>
          <p>Instagram</p>
        </a>
      </li>
      <li class='icon col-md-2'>
        <a href='https://twitter.com/CLondenMusic'>
          <font-awesome-icon :icon="twitter"/>
          <p>Twitter</p>
        </a>
      </li>
      <li class='icon col-md-2'>
        <a>
          <font-awesome-icon :icon="snapchat"/>
          <p>Snapchat</p>
        </a>
      </li>
      <li class='icon col-md-2'>
        <a>
          <font-awesome-icon :icon="youtube"/>
          <p>Youtube</p>
        </a>
      </li>
    </ul>
  </div>
</template>

<script>
import FontAwesomeIcon from '@fortawesome/vue-fontawesome'
import faFacebook from '@fortawesome/fontawesome-free-brands/faFacebook'
import faInstagram from '@fortawesome/fontawesome-free-brands/faInstagram'
import faSnapchatsquare from '@fortawesome/fontawesome-free-brands/faSnapchat'
import faTwittersquare from '@fortawesome/fontawesome-free-brands/faTwitter'
import faYoutube from '@fortawesome/fontawesome-free-brands/faYoutube'

export default {
  name: 'MyFooter',
  computed: {
    facebook () {
      return faFacebook
    },
    instagram () {
      return faInstagram
    },
    snapchat () {
      return faSnapchatsquare
    },
    twitter () {
      return faTwittersquare
    },
    youtube () {
      return faYoutube
    }
  },
  components: {
    FontAwesomeIcon
  }
}
</script>

<style lang='scss'>
  @import '../../src/assets/sass/now-ui-kit.scss';
</style>
