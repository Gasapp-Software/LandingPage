<template>
  <div>
    <!-- Hero phrase start -->
    <home-hero />
    <!-- Hero phrase end -->
    <!-- Value proposition start -->
    <home-value />
    <!-- Value proposition end -->
    <home-order />

    <home-dispatchers />

    <home-business />

    <bottom />
  </div>
</template>

<script>
import observer from '~/assets/mixins/Observer'
export default {
  mixins: [observer],
  layout: 'Main',
  transition: {
    name: 'zoom',
    mode: 'out-in',
  },
  data() {
    return {}
  },
}
</script>

<style>
.nuxt-content ul li {
  @apply mb-5 relative pl-5;
}
.nuxt-content ul li::before {
  content: '▹';
  @apply text-primary-400 top-0 left-0 absolute text-base;
}

.nuxt-content a {
  @apply text-primary-600 hover:text-primary-900;
}
</style>
