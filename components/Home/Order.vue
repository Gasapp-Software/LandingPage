<template>
  <section class="px-6 pt-20 pb-20">
    <div
      class="max-w-5xl mx-auto order-bg px-6 py-14 border shadow-lg rounded-3xl"
    >
      <h2
        class="
          mx-auto
          text-center
          md:text-7xl
          mb-10
          text-5xl
          font-bold
          text-gray-800
          md:w-7/12
          hide-slideUp
        "
      >
        Making an order is super <span class="text-primary-600">easy</span>
      </h2>
      <div class="flex justify-between items-center flex-wrap">
        <div class="w-full mb-3 lg:w-3/12 hide-slideInLeft">
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
              text-center text-red-500 text-bold
              font-mono
            "
          >
            {{ steps[defaultStepIndex].step }}
          </p>
        </div>
        <div class="w-full mb-6 lg:w-4/12">
          <div class="w-8/12 mx-auto hide-slideUp">
            <phone :screens="phoneScreens" @indexChange="changeIndex($event)" />
          </div>
        </div>
        <div class="w-full lg:w-3/12 hide-slideInRight">
          <p
            class="
              text-center
              lg:text-left
              md:text-4xl
              mb-5
              text-2xl
              font-bold
              text-gray-600
            "
          >
            {{ steps[defaultStepIndex].instruction }}
          </p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      defaultStepIndex: 0,
      phoneScreens: [
        '/phone_screens/customer/1.png',
        '/phone_screens/customer/2.png',
        '/phone_screens/customer/3.png',
        '/phone_screens/customer/4.png',
        '/phone_screens/customer/5.png',
        '/phone_screens/customer/6.png',
      ],
      steps: [
        {
          step: '01',
          instruction: 'Login to Gasapp',
        },
        {
          step: '02',
          instruction: 'Enter quantity of product to be ordered',
        },
        {
          step: '03',
          instruction: 'Find vendor and dispatcher',
        },
        {
          step: '04',
          instruction: 'Select payment method',
        },
        {
          step: '05',
          instruction: 'Confirm order',
        },
        {
          step: '06',
          instruction: 'Wait for Dispatcher',
        },
      ],
    }
  },
  methods: {
    changeIndex(e) {
      this.defaultStepIndex = e
    },
  },
}
</script>

<style scoped>
@import '@/components/Home/Home.css';
</style>
