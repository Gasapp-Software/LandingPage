<template>
  <section class="px-6 pt-20 pb-20">
    <div class="max-w-5xl mx-auto flex justify-between flex-wrap">
      <div class="w-full lg:w-4/12">
        <h2
          class="
            text-5xl
            md:text-7xl
            text-center
            md:text-left
            font-bold
            text-gray-900
            hide-slideUp
          "
        >
          <span class="text-primary-600">Value</span> assured
        </h2>
        <div class="mt-10 w-full">
          <figure
            class="
              w-full
              hide-slideUp
              block
              h-80
              bg-gray-800
              rounded-2xl
              overflow-hidden
            "
          >
            <img
              src="/value.jpg"
              class="w-full h-full object-cover object-right-bottom"
              alt="Gasapp value services"
            />
          </figure>
        </div>
      </div>
      <div
        class="
          w-full
          mt-10
          lg:mt-0
          grid grid-col-1
          gap-6
          md:grid-cols-2
          lg:w-6/12
        "
      >
        <div class="hide-slideUp">
          <figure class="mb-3 w-24 h-auto">
            <img
              class="w-full"
              src="/services/speed.svg"
              alt="lightspeed delivery"
            />
          </figure>
          <h3 class="text-base font-bold text-gray-800 mb-3">
            Lightspeed Delivery
          </h3>
          <p class="text-gray-500 text-sm">
            When you make an order, we ensure you have your fuel gets delivered
            to you before you even think of reaching for the clock
          </p>
        </div>
        <div class="hide-slideUp">
          <figure class="mb-3 w-24 h-auto">
            <img
              class="w-full"
              src="/services/options.svg"
              alt="lightspeed delivery"
            />
          </figure>
          <h3 class="text-base font-bold text-gray-800 mb-3">Order Choice</h3>
          <p class="text-gray-500 text-sm">
            We are called Gasapp but not limited to the delivery of gas orders.
            You can make order for other available petroleum products such as
            petrol, kerosene and diesel
          </p>
        </div>
        <div class="hide-slideUp">
          <figure class="mb-3 w-24 h-auto">
            <img
              class="w-full"
              src="/services/vendor.svg"
              alt="lightspeed delivery"
            />
          </figure>
          <h3 class="text-base font-bold text-gray-800 mb-3">
            Trusted Vendors
          </h3>
          <p class="text-gray-500 text-sm">
            Gasapp has a plethora of trusted businesses onboard who are always
            ready to take your orders and ensure you get the best quality of
            petroleum products your money can buy.
          </p>
        </div>
        <div class="hide-slideUp">
          <figure class="mb-3 w-24 h-auto">
            <img
              class="w-full"
              src="/services/dispatcher.svg"
              alt="lightspeed delivery"
            />
          </figure>
          <h3 class="text-base font-bold text-gray-800 mb-3">
            Reliable Dispatchers
          </h3>
          <p class="text-gray-500 text-sm">
            We employ the services of well scrutinized and experienced dispatch
            riders to ensure your orders reach your door step on time and in one
            piece
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
