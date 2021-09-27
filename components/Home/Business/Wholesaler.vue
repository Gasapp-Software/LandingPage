<template>
  <div
    id="wholesaler"
    class="
      flex
      mt-24
      flex-wrap
      md:flex-row-reverse
      w-full
      items-stretch
      justify-center
    "
  >
    <div class="w-full md:w-6/12 mb-10 md:mb-0">
      <div
        class="w-8/12 md:w-6/12 mx-auto md:mx-0 md:ml-auto hide-slideInRight"
      >
        <phone :screens="phoneScreens" />
      </div>
    </div>
    <div class="w-full md:w-4/12">
      <div class="mb-10">
        <p
          class="
            inline-flex
            items-center
            px-4
            py-1
            border
            text-xs
            mb-3
            rounded-full
            border-primary-300
            text-primary-600
            font-bold
            hide-slideUp
          "
        >
          Gasapp Wholesaler
          <img
            src="/icons/petroleum.svg"
            class="w-6 ml-3"
            alt="gasapp wholesaler icon"
          />
        </p>
        <p class="text-base md:text-lg text-gray-800 mb-3 hide-slideInRight">
          Wholesale businesses consist of filling stations and gas stations that
          sell petroleum products in large scale
        </p>
        <p class="text-base md:text-lg text-gray-800 hide-slideInRight">
          You are eligible to be a Gasapp wholesaler if :
        </p>
        <div class="mt-5">
          <div class="flex items-center mb-3 text-gray-700 hide-slideInRight">
            <span class="icon-check bg-primary-100 text-primary-600">
              <check-icon size="1x" />
            </span>
            <div class="ml-3 w-10/12 text-sm">
              You are a registered business under the CAC
            </div>
          </div>
          <div class="flex items-center mb-3 text-gray-700 hide-slideInRight">
            <span class="icon-check bg-primary-100 text-primary-600">
              <check-icon size="1x" />
            </span>
            <div class="ml-3 w-10/12 text-sm">
              You have a verifiable business address
            </div>
          </div>
          <div class="flex items-center mb-3 text-gray-700 hide-slideInRight">
            <span class="icon-check bg-primary-100 text-primary-600">
              <check-icon size="1x" />
            </span>
            <div class="ml-3 w-10/12 text-sm">
              You have a valid contact information
            </div>
          </div>
        </div>
      </div>
      <div>
        <p class="text-base md:text-lg text-gray-800 mb-5 hide-slideInRight">
          Start your registration by downloading our wholesaler app.
        </p>
        <download-btn></download-btn>
      </div>
    </div>
  </div>
</template>

<script>
import { CheckIcon } from 'vue-feather-icons'

export default {
  components: {
    CheckIcon,
  },
  data() {
    return {
      phoneScreens: [
        '/phone_screens/wholesaler/1.png',
        '/phone_screens/wholesaler/2.png',
      ],
    }
  },
}
</script>

<style scoped>
@import '@/components/Home/Home.css';
</style>
