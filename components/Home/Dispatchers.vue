<template>
  <section class="px-6 pt-20 pb-20">
    <div class="max-w-5xl mx-auto flex justify-between flex-wrap">
      <h2
        class="
          w-full
          md:w-6/12
          mx-auto
          text-5xl text-center
          md:text-8xl
          outlined-text
          secondary
          hide-slideUp
        "
      >
        Earn as a Dispatcher
      </h2>
      <div class="flex mt-10 flex-wrap w-full items-stretch justify-center">
        <div class="w-full md:w-6/12 mb-10 md:mb-0">
          <div
            class="w-8/12 md:w-6/12 mx-auto md:mx-0 md:mr-auto hide-slideInLeft"
          >
            <phone :screens="phoneScreens" />
          </div>
        </div>
        <div class="w-full md:w-4/12">
          <div class="mb-10">
            <p
              class="
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
                inline-flex
                justify-between
                items-center
              "
            >
              <span>Gasapp Dispatcher</span>
              <img
                src="/icons/truck.svg"
                class="w-6 ml-3"
                alt="gasapp dispatcher icon"
              />
            </p>
            <p
              class="text-base md:text-lg text-gray-700 mb-3 hide-slideInRight"
            >
              Register as a Gasapp Dispatcher and get paid per delivery you
              complete.
            </p>
            <p class="text-base md:text-lg text-gray-700 hide-slideInRight">
              You are eligible to be Gasapp dispatch rider if ;
            </p>
            <div class="mt-5">
              <div
                class="flex items-center mb-3 text-gray-500 hide-slideInRight"
              >
                <span class="icon-check bg-primary-100 text-primary-600">
                  <check-icon size="1x" />
                </span>
                <div class="ml-3 w-10/12 text-sm">
                  You are above 18 years age
                </div>
              </div>
              <div
                class="flex items-center mb-3 text-gray-500 hide-slideInRight"
              >
                <span class="icon-check bg-primary-100 text-primary-600">
                  <check-icon size="1x" />
                </span>
                <div class="ml-3 w-10/12 text-sm">
                  You have a vehicle (wagon, minibus, or pickup)
                </div>
              </div>
              <div
                class="flex items-center mb-3 text-gray-500 hide-slideInRight"
              >
                <span class="icon-check bg-primary-100 text-primary-600">
                  <check-icon size="1x" />
                </span>
                <div class="ml-3 w-10/12 text-sm">
                  You have a valid driver's licence
                </div>
              </div>
            </div>
          </div>
          <div>
            <p
              class="text-base md:text-lg text-gray-700 mb-5 hide-slideInRight"
            >
              Start your registration by downloading our dispatcher app.
            </p>
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
        </div>
      </div>
    </div>
  </section>
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
        '/phone_screens/dispatcher/1.png',
        '/phone_screens/dispatcher/2.png',
        '/phone_screens/dispatcher/3.png',
        '/phone_screens/dispatcher/4.png',
      ],
    }
  },
}
</script>

<style scoped>
@import '@/components/Home/Home.css';
</style>
