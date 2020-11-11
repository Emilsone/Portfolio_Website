<template>
  <div class="logo-image">
    <img src="~/assets/img/logo.png" class="" alt="" />
  </div>
</template>

<script>
export default {
  name: 'Logo',
  props: {
    isStickable: {
      type: Boolean,
      default: false
    },
    isSticky: {
      type: Boolean,
      default: false
    }
  },
  computed: {
    classList() {
      let classList = ''
      if (this.isStickable) {
        classList = this.isSticky ? 'text-gray-800' : 'text-white'
      } else {
        classList = 'text-orange-600'
      }
      return classList
    }
  }
}
</script>
