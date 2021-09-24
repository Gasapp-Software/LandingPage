<template>
  <section class="px-6 pt-20 pb-20">
    <div
      class="max-w-5xl mx-auto order-bg px-6 py-14 border shadow-lg rounded-3xl"
    >
      <h2
        class="
          mx-auto
          text-center
          md:text-6xl
          mb-10
          text-5xl
          font-bold
          text-gray-800
          md:w-6/12
        "
      >
        Making an order is super easy
      </h2>
      <div class="flex justify-between items-center flex-wrap">
        <div class="w-full mb-3 lg:w-3/12">
          <span
            class="
              block
              text-center
              mx-auto
              w-14
              py-2
              px-4
              border
              text-gray-500 text-sm
              rounded-full
              border-gray-300
            "
            >Step
          </span>
          <p
            class="
              text-5xl
              md:text-8xl
              text-center
              outlined-text
              secondary
              font-mono
            "
          >
            01
          </p>
        </div>
        <div class="w-full mb-6 lg:w-4/12">
          <div class="w-8/12 mx-auto">
            <phone />
          </div>
        </div>
        <div class="w-full lg:w-3/12">
          <p
            class="
              text-center
              md:text-left md:text-4xl
              mb-5
              text-2xl
              font-bold
              text-gray-600
            "
          >
            Login to Gasapp
          </p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {}
</script>

<style scoped>
@import '@/components/Home/Home.css';
</style>
