<template>
  <section class="text-gray-700">
    <div class="container px-5 py-24 mx-auto">
      <TabIndex @tabchange="changeTab($event)" />
      <div class="general-container" v-show="tabActiveIndex == 0">
        <div class="flex flex-wrap justify-center -m-4">
          <div class="p-4 lg:w-2/5">
            <div
              class="h-full px-8 pt-16 pb-24 overflow-hidden  relative card-page"
            >
              <h1
                class="title-font sm:text-2xl text-xl font-medium text-white mb-3"
              >
                Payme Design System
              </h1>
              <p class="leading-relaxed mb-3">
                MyCustomer is an on-demand, scalable ledger solution for small
                and medium sized businesses globally.
              </p>
              <a class="text-indigo-500 inline-flex items-center"
                >Read Case Study
                <svg
                  class="w-4 h-4 ml-2"
                  viewBox="0 0 24 24"
                  stroke="currentColor"
                  stroke-width="2"
                  fill="none"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                >
                  <path d="M5 12h14"></path>
                  <path d="M12 5l7 7-7 7"></path>
                </svg>
              </a>
              <div class=" mt-24 flex   ">
                <img
                  src="~/assets/img/holding-iphone.png"
                  alt=" love logo"
                  class="ml-auto image-phone"
                  id="image-phone"
                />
              </div>
            </div>
          </div>
          <div class="p-4 lg:w-2/5">
            <div
              class="h-full  px-8 pt-16 pb-24  overflow-hidden  relative card-page"
            >
              <h1
                class="title-font sm:text-2xl text-xl font-medium text-white mb-3"
              >
                Payme Design System
              </h1>
              <p class="leading-relaxed mb-3">
                MyCustomer is an on-demand, scalable ledger solution for small
                and medium sized businesses globally.
              </p>
              <a class="text-indigo-500 inline-flex items-center"
                >Real Case Study
                <svg
                  class="w-4 h-4 ml-2"
                  viewBox="0 0 24 24"
                  stroke="currentColor"
                  stroke-width="2"
                  fill="none"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                >
                  <path d="M5 12h14"></path>
                  <path d="M12 5l7 7-7 7"></path>
                </svg>
              </a>
              <div class=" mt-24 flex   ">
                <img
                  src="~/assets/img/holding-iphone.png"
                  alt=" love logo"
                  class="ml-auto image-phone"
                  id="image-phone"
                />
              </div>
            </div>
          </div>
        </div>
        <!-- end of card page -->
        <div class="flex flex-wrap justify-center -m-4">
          <div class="p-4 lg:w-2/5">
            <div
              class="h-full bg-gray-200 px-8 pt-16 pb-24  overflow-hidden  relative card-two"
            >
              <h1
                class="title-font sm:text-2xl  text-xl font-medium text-gray-900 mb-3"
              >
                Payme Design System
              </h1>
              <p class="leading-relaxed mb-3">
                MyCustomer is an on-demand, scalable ledger solution for small
                and medium sized businesses globally.
              </p>
              <a class="text-indigo-500 inline-flex items-center"
                >Real Case Study
                <svg
                  class="w-4 h-4 ml-2"
                  viewBox="0 0 24 24"
                  stroke="currentColor"
                  stroke-width="2"
                  fill="none"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                >
                  <path d="M5 12h14"></path>
                  <path d="M12 5l7 7-7 7"></path>
                </svg>
              </a>
              <div class=" mt-24 flex   ">
                <img
                  src="~/assets/img/holding-iphone.png"
                  alt=" love logo"
                  class="ml-auto image-phone"
                  id="image-phone"
                />
              </div>
            </div>
          </div>
          <div class="p-4 lg:w-2/5">
            <div
              class="h-full bg-gray-200 px-8 pt-16 pb-24 overflow-hidden  relative card-two"
            >
              <h1
                class="title-font sm:text-2xl  text-xl font-medium text-gray-900 mb-3"
              >
                Payme Design System
              </h1>
              <p class="leading-relaxed mb-3">
                MyCustomer is an on-demand, scalable ledger solution for small
                and medium sized businesses globally.
              </p>
              <a class="text-indigo-500 inline-flex items-center"
                >Real Case Study
                <svg
                  class="w-4 h-4 ml-2"
                  viewBox="0 0 24 24"
                  stroke="currentColor"
                  stroke-width="2"
                  fill="none"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                >
                  <path d="M5 12h14"></path>
                  <path d="M12 5l7 7-7 7"></path>
                </svg>
              </a>
              <div class=" mt-24 flex   ">
                <img
                  src="~/assets/img/holding-iphone.png"
                  alt=" love logo"
                  class="ml-auto image-phone"
                  id="image-phone"
                />
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="digital-container " v-show="tabActiveIndex == 1">
        <DigitalMarketing />
      </div>
      <div class="logo-container" v-show="tabActiveIndex == 2">
        <LogoContent />
      </div>
    </div>
  </section>
</template>
<script>
import TabIndex from "@/components/TabIndex.vue";
import LogoContent from "@/components/LogoContent.vue";
import DigitalMarketing from "@/components/DigitalMarketing.vue";
export default {
  name: "Projects",
  components: {
    TabIndex,
    DigitalMarketing,
    LogoContent,
  },
  data() {
    return {
      tabActiveIndex: 0,
    };
  },
  methods: {
    changeTab(val) {
      this.tabActiveIndex = val;
    },
  },
};
</script>
<style>
.card-page {
  background-color: #012b3d;
}
.card-two {
  background-color: #d9f6f1;
}
.work-heading {
  padding-left: 20px;
}
/* .iphone-pro img{
  width:280px;
  height:280px;
} */
</style>
