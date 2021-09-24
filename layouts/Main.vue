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
          <a class="w-32 inline-block font-bold mr-4 md:mr-14">
            <img src="/gasapp_logo.svg" alt="Gasapp Logo" />
          </a>
          <nav v-if="isHomePage === true" class="flex items-center text-sm">
            <ul class="md:flex text-gray-600 items-center mr-4 hidden">
              <li class="mr-9">
                <a href="#about" class="hover:text-primary-500">Dispatchers</a>
              </li>
              <li class="mr-9">
                <a href="#portfolio" class="hover:text-primary-500">Vendors</a>
              </li>
              <li class="mr-9">
                <a href="#work" class="hover:text-primary-500">Customers</a>
              </li>
              <!-- <li class="mr-9">
              <a href="#contact" class="hover:text-primary-500">Contact</a>
            </li> -->
            </ul>
          </nav>
        </div>
        <action-e-link
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
          <a href="#about" class="text-gray-700 hover:text-primary-500"
            >Customers</a
          >
        </li>
        <li class="inline-block w-auto mr-7">
          <a href="#portfolio" class="text-gray-700 hover:text-primary-500"
            >Dispatcher</a
          >
        </li>
        <li class="inline-block w-auto mr-7">
          <a href="#work" class="text-gray-700 hover:text-primary-500"
            >Businesses</a
          >
        </li>
      </ul>
    </aside>
    <nuxt-child />
    <footer></footer>
    <socials />
    <email-comp />
  </div>
</template>
<script>
export default {
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
