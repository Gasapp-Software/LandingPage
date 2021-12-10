<template>
  <footer id="contact" class="px-6 pt-20 z-10">
    <div class="max-w-5xl mx-auto flex justify-between flex-wrap">
      <div class="mb-10 w-full rounded-2xl overflow-hidden">
        <div
          class="
            py-10
            footer-bg
            px-10
            flex flex-wrap
            md:flex-nowrap
            justify-between
            items-center
          "
        >
          <h2
            class="md:text-7xl font-bold w-full md:w-6/12 text-5xl text-white"
          >
            Give <span class="text-primary-600">Gas</span
            ><span class="text-red-500">app</span> a try today
          </h2>
          <div class="mt-10 md:mt-0 w-full md:w-auto inline-block">
            <download-btn />
          </div>
        </div>
        <div
          class="
            py-20
            bg-gray-900
            px-10
            grid grid-cols-1
            md:grid-cols-2
            lg:grid-cols-4
            gap-4
          "
        >
          <div>
            <h4 class="text-xs uppercase tracking-widest text-gray-200 mb-3">
              Address
            </h4>
            <p class="text-sm text-gray-400">
              Lorem, ipsum dolor sit amet consectetur adipisicing elit.
              Reprehenderit vero, tenetur consequuntur
            </p>
          </div>
          <div>
            <h4 class="text-xs uppercase tracking-widest text-gray-200 mb-3">
              Email
            </h4>
            <a
              href="mailto:support@gasapp.company"
              class="text-sm text-gray-400 hover:text-gray-300"
            >
              support@gasapp.company
            </a>
          </div>
          <div>
            <h4 class="text-xs uppercase tracking-widest text-gray-200 mb-3">
              Phone
            </h4>
            <ul>
              <li class="mb-2">
                <a
                  href="tel:2348061410220"
                  class="text-sm text-gray-400 hover:text-gray-300"
                >
                  +2348061410220
                </a>
              </li>
            </ul>
          </div>
          <div>
            <h4 class="text-xs uppercase tracking-widest text-gray-200 mb-3">
              Social
            </h4>
            <ul class="flex items-center flex-wrap">
              <li class="mr-4 mb-3">
                <a href="#" class="text-sm text-gray-400 hover:text-gray-300">
                  <facebook-icon size="1.5x" />
                </a>
              </li>
              <li class="mr-4 mb-3">
                <a href="#" class="text-sm text-gray-400 hover:text-gray-300">
                  <twitter-icon size="1.5x" />
                </a>
              </li>
              <li class="mr-4 mb-3">
                <a href="#" class="text-sm text-gray-400 hover:text-gray-300">
                  <linkedin-icon size="1.5x" />
                </a>
              </li>
              <li class="mr-4 mb-3">
                <a href="#" class="text-sm text-gray-400 hover:text-gray-300">
                  <instagram-icon size="1.5x" />
                </a>
              </li>
            </ul>
          </div>
        </div>
      </div>
      <div class="flex w-full flex-wrap justify-between">
        <div class="w-full md:w-auto inline-block mb-5 md:mb-0">
          <a id="#home" class="w-32 inline-block font-bold mr-4 md:mr-14">
            <img src="/gasapp_logo.svg" alt="Gasapp Logo" />
          </a>
          <p class="text-sm text-gray-600">Gasapp © {{ getYear() }}</p>
        </div>
        <ul class="flex items-center">
          <li class="mr-4 mb-2 md:mb-0">
            <a
              href="#"
              class="text-sm text-gray-600 hover:text-gray-800 capitalize"
              >Careers</a
            >
          </li>
          <li class="mr-4 mb-2 md:mb-0">
            <a
              href="#"
              class="text-sm text-gray-600 hover:text-gray-800 capitalize"
              >Terms & Conditions</a
            >
          </li>
          <li class="mr-4 mb-2 md:mb-0">
            <nuxt-link
              to="/privacy_policy"
              class="text-sm text-gray-600 hover:text-gray-800 capitalize"
              >Privacy Policy</nuxt-link
            >
          </li>
        </ul>
      </div>
    </div>
  </footer>
</template>

<script>
import {
  TwitterIcon,
  FacebookIcon,
  LinkedinIcon,
  InstagramIcon,
} from 'vue-feather-icons'
export default {
  components: {
    TwitterIcon,
    FacebookIcon,
    LinkedinIcon,
    InstagramIcon,
  },
  methods: {
    getYear() {
      return new Date().getFullYear()
    },
  },
}
</script>

<style>
.footer-bg {
  background-color: #313333;
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='100%25' height='100%25' viewBox='0 0 1600 800'%3E%3Cg %3E%3Cpath fill='%232b2c2c' d='M486 705.8c-109.3-21.8-223.4-32.2-335.3-19.4C99.5 692.1 49 703 0 719.8V800h843.8c-115.9-33.2-230.8-68.1-347.6-92.2C492.8 707.1 489.4 706.5 486 705.8z'/%3E%3Cpath fill='%23252626' d='M1600 0H0v719.8c49-16.8 99.5-27.8 150.7-33.5c111.9-12.7 226-2.4 335.3 19.4c3.4 0.7 6.8 1.4 10.2 2c116.8 24 231.7 59 347.6 92.2H1600V0z'/%3E%3Cpath fill='%231f1f1f' d='M478.4 581c3.2 0.8 6.4 1.7 9.5 2.5c196.2 52.5 388.7 133.5 593.5 176.6c174.2 36.6 349.5 29.2 518.6-10.2V0H0v574.9c52.3-17.6 106.5-27.7 161.1-30.9C268.4 537.4 375.7 554.2 478.4 581z'/%3E%3Cpath fill='%23181818' d='M0 0v429.4c55.6-18.4 113.5-27.3 171.4-27.7c102.8-0.8 203.2 22.7 299.3 54.5c3 1 5.9 2 8.9 3c183.6 62 365.7 146.1 562.4 192.1c186.7 43.7 376.3 34.4 557.9-12.6V0H0z'/%3E%3Cpath fill='%23121212' d='M181.8 259.4c98.2 6 191.9 35.2 281.3 72.1c2.8 1.1 5.5 2.3 8.3 3.4c171 71.6 342.7 158.5 531.3 207.7c198.8 51.8 403.4 40.8 597.3-14.8V0H0v283.2C59 263.6 120.6 255.7 181.8 259.4z'/%3E%3Cpath fill='%231f1f1f' d='M1600 0H0v136.3c62.3-20.9 127.7-27.5 192.2-19.2c93.6 12.1 180.5 47.7 263.3 89.6c2.6 1.3 5.1 2.6 7.7 3.9c158.4 81.1 319.7 170.9 500.3 223.2c210.5 61 430.8 49 636.6-16.6V0z'/%3E%3Cpath fill='%232d2d2d' d='M454.9 86.3C600.7 177 751.6 269.3 924.1 325c208.6 67.4 431.3 60.8 637.9-5.3c12.8-4.1 25.4-8.4 38.1-12.9V0H288.1c56 21.3 108.7 50.6 159.7 82C450.2 83.4 452.5 84.9 454.9 86.3z'/%3E%3Cpath fill='%233a3a3a' d='M1600 0H498c118.1 85.8 243.5 164.5 386.8 216.2c191.8 69.2 400 74.7 595 21.1c40.8-11.2 81.1-25.2 120.3-41.7V0z'/%3E%3Cpath fill='%23484848' d='M1397.5 154.8c47.2-10.6 93.6-25.3 138.6-43.8c21.7-8.9 43-18.8 63.9-29.5V0H643.4c62.9 41.7 129.7 78.2 202.1 107.4C1020.4 178.1 1214.2 196.1 1397.5 154.8z'/%3E%3Cpath fill='%23555555' d='M1315.3 72.4c75.3-12.6 148.9-37.1 216.8-72.4h-723C966.8 71 1144.7 101 1315.3 72.4z'/%3E%3C/g%3E%3C/svg%3E");
  background-attachment: fixed;
  background-size: cover;
}
</style>
