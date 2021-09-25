<template>
  <section class="px-6 pt-20 md:pt-40 pb-20 relative z-10">
    <div class="max-w-5xl mx-auto flex justify-between flex-wrap">
      <div class="w-full lg:mr-10 lg:w-6/12">
        <h1
          class="md:text-6xl text-5xl font-bold text-gray-800 hide-slideInRight"
        >
          <span class="text-red-500">Gas</span> purchase with just a simple
          click
        </h1>
        <p class="mt-3 text-sm lg:text-base text-gray-600 hide-slideInRight">
          Gasapp reduces the stress of leaving your home to purchase fuel by
          enabling you order for fuel from the comfort of your home with just
          few clicks on your mobile device
        </p>
        <div
          class="
            rounded-3xl
            lg:rounded-full
            mt-10
            p-2
            w-full
            lg:w-auto
            border border-gray-300
            inline-flex
            flex-wrap
            items-center
            hide-slideUp
          "
        >
          <action-e-link
            :extra-css="[
              'btn-dark',
              'lg:mr-3',
              'w-full',
              'lg:w-auto',
              'mb-3',
              'lg:mb-0',
              'btn-rounded',
            ]"
          >
            <div class="w-5 mr-4">
              <img class="w-full" src="/playstore.svg" alt="" />
            </div>
            <div>
              <div class="text-xs text-gray-500">Available on</div>
              <div class="text-white text-sm">Play store</div>
            </div>
          </action-e-link>
          <action-e-link
            :extra-css="['btn-dark', 'btn-rounded', 'w-full', 'lg:w-auto']"
          >
            <div class="w-6 mr-4">
              <img class="w-full" src="/apple.svg" alt="" />
            </div>
            <div>
              <div class="text-xs text-gray-500">Available on</div>
              <div class="text-white text-sm">App store</div>
            </div>
          </action-e-link>
        </div>
      </div>
      <div class="w-full mt-10 lg:mt-0 lg:w-4/12">
        <div class="w-8/12 mx-auto hide-slideUp">
          <phone />
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {}
</script>

<style></style>
