<template>
  <main class="px-6 pb-20 relative z-10">
    <section
      class="max-w-5xl mx-auto flex py-20 md:py-40 justify-between flex-wrap"
    >
      <div class="w-full lg:mr-10 lg:w-6/12">
        <h1
          class="md:text-7xl text-5xl font-bold text-gray-800 hide-slideInRight"
        >
          Terms and <br />
          <span class="text-red-500">Conditions</span>
        </h1>
        <p class="mt-3 text-sm lg:text-base text-gray-500 hide-slideInRight">
          Please read carefully our Termsof Service Before Placing an order on
          GasApp Africa. By ordering Gas from Werblo’s Gas App Africa through
          the Mobile App you agree to be bound by these Terms and Conditions.
        </p>
      </div>
    </section>
    <section class="max-w-5xl mx-auto pt-20 md:pt-52">
      <nuxt-content :document="terms" />
    </section>
  </main>
</template>

<script>
import observer from '~/assets/mixins/Observer'
export default {
  mixins: [observer],
  layout: 'Main',
  async asyncData({ $content }) {
    const terms = await $content('terms_and_conditions').fetch()
    return {
      terms,
    }
  },
}
</script>

<style>
.nuxt-content section {
  @apply py-20;
}

.nuxt-content p {
  @apply text-gray-700;
}

.nuxt-content h1,
.nuxt-content h2,
.nuxt-content h3,
.nuxt-content h4 {
  @apply mb-3 mt-5 font-bold;
}

.nuxt-content h1 {
  @apply text-3xl text-primary-600;
}

.nuxt-content article {
  @apply bg-gray-200 rounded-xl px-6 py-4 border border-gray-500 my-6;
}

@screen md {
  .nuxt-content h1 {
    @apply text-6xl;
  }
}
</style>
