<template>
  <div>
    <div
      class="border-8 border-black rounded-3xl relative"
      style="aspect-ratio: 6 / 13"
    >
      <div class="h-1/6 bg-black w-2 absolute top-6 -left-3"></div>
      <div class="w-full z-10 absolute bottom-0 p-2">
        <span
          class="block mx-auto w-4/12 rounded-full border-2 border-black"
        ></span>
      </div>
      <div class="w-full bg-white rounded-2xl overflow-hidden h-full">
        <transition name="zoom" mode="out-in">
          <template v-for="(screen, index) in screens">
            <img
              v-if="index === defaultScreenIndex"
              :key="index"
              :src="screen"
              class="w-full h-auto"
              alt=""
              :draggable="false"
            />
          </template>
        </transition>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    screens: {
      type: Array,
      default() {
        return [
          '/phone_screens/home_screen.png',
          '/phone_screens/finding_retailers.png',
          '/phone_screens/found.png',
        ]
      },
    },
    canChange: {
      type: Boolean,
      default: true,
    },
  },
  data() {
    return {
      defaultScreenIndex: 0,
    }
  },
  mounted() {
    const triggerChange = () => {
      setTimeout(() => {
        this.changeScreenIndex()
        return triggerChange()
      }, 3000)
    }
    if (this.canChange === true) triggerChange()
  },
  methods: {
    changeScreenIndex() {
      if (this.defaultScreenIndex === this.screens.length - 1)
        return (this.defaultScreenIndex = 0)
      return (this.defaultScreenIndex += 1)
    },
  },
}
</script>

<style></style>
