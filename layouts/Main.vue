<template>
  <div class="font-sans relative pb-20 md:pb-10">
    <div
      class="w-full flex justify-between absolute top-0"
      style="height: 720px"
    >
      <div class="hidden lg:block lg:w-6/12 h-full"></div>
      <div
        class="hidden lg:block lg:w-5/12 h-full hero-pattern rounded-bl-2xl"
      ></div>
    </div>
    <header class="w-full md:absolute top-0 left-0 z-20">
      <div
        class="
          px-4
          lg:px-0
          max-w-5xl
          mx-auto
          flex
          items-center
          justify-between
          py-3
        "
      >
        <div class="flex items-center">
          <nuxt-link to="/" class="w-32 inline-block font-bold mr-4 md:mr-14">
            <img src="/gasapp_logo.svg" alt="Gasapp Logo" />
          </nuxt-link>
          <nav class="flex items-center text-sm">
            <ul class="md:flex text-gray-600 items-center mr-4 hidden">
              <li class="mr-9">
                <a href="#dispatcher" class="hover:text-primary-500"
                  >Dispatchers</a
                >
              </li>
              <li class="mr-9">
                <a href="#vendor" class="hover:text-primary-500">Vendors</a>
              </li>
            </ul>
          </nav>
        </div>
        <action-e-link
          href="#contact"
          :extra-css="['btn-primary__light', 'text-sm', 'btn-rounded']"
          >Contact us</action-e-link
        >
      </div>
    </header>
    <aside
      v-if="isHomePage === true"
      class="md:hidden block navbar fixed w-full bottom-0 left-0 z-20"
    >
      <ul
        class="
          max-w-5xl
          px-4
          md:px-0
          mx-auto
          md:hidden
          items-center
          py-4
          border-b-1
          text-xs
          flex
          justify-center
          overflow-x-auto
        "
      >
        <li class="inline-block w-auto mr-7">
          <a href="#dispatcher" class="text-gray-700 hover:text-primary-500"
            >Dispatcher</a
          >
        </li>
        <li class="inline-block w-auto mr-7">
          <a href="#retailer" class="text-gray-700 hover:text-primary-500"
            >Retailers</a
          >
        </li>
        <li class="inline-block w-auto">
          <a href="#wholesaler" class="text-gray-700 hover:text-primary-500"
            >Wholesalers</a
          >
        </li>
      </ul>
    </aside>
    <nuxt-child />
    <bottom />
    <!-- <socials />
    <email-comp /> -->
  </div>
</template>
<script>
export default {
  head: {
    script: [
      {
        src: '/jsServices/crispChat.js',
        async: true,
        defer: true,
      },
    ],
  },
  computed: {
    isHomePage() {
      return this.$route.name === 'index'
    },
  },
}
</script>
<style scoped>
@import '@/layouts/Layout.css';
</style>
