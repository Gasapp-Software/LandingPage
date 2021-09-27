<template>
  <div
    class="
      rounded-3xl
      lg:rounded-full
      p-2
      w-full
      lg:w-auto
      border border-gray-300
      inline-flex
      flex-wrap
      lg:flex-nowrap
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
</template>

<script>
export default {}
</script>

<style></style>
