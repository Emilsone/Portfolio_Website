<template>
  <header class="text-gray-700 body-font">
    <div
      class="container mx-auto flex flex-wrap p-5 flex-col md:flex-row items-center"
    >
      <a
        class="flex title-font font-medium items-center text-gray-900 mb-4 md:mb-0"
      >
        <span class="pl-24 text-xl">tailblocks</span>
      </a>
      <nav
        class="md:ml-auto flex flex-wrap items-center text-base justify-center"
      >
        <a
          class="mr-5  tab"
          :class="{ active: tabActiveIndex == 0 }"
          @click="changeTab(0)"
          >Ui Design</a
        >
        <a
          class="mr-5  tab"
          :class="{ active: tabActiveIndex == 1 }"
          @click="changeTab(1)"
          >Digital Design</a
        >
        <a
          class="mr-5  tab"
          :class="{ active: tabActiveIndex == 2 }"
          @click="changeTab(2)"
          >Logo</a
        >
        <!-- <a class="mr-5 hover:text-gray-900">Fourth Link</a> -->
      </nav>
    </div>
  </header>
</template>
<script>
export default {
  name: "TabIndex",
  data() {
    return {
      tabActiveIndex: 0,
    };
  },
  methods: {
    changeTab(val) {
      this.tabActiveIndex = val;
      this.$emit("tabchange", this.tabActiveIndex);
    },
  },
};
</script>
<style>
.tab {
  height: 100%;
  text-align: center;
  flex: 1;
  display: flex;
  align-items: center;
  justify-content: center;
  cursor: pointer;
  border-bottom: 1px solid rgba(128, 128, 128, 0.53);
  --active-color: #ff0000;
}

.tab.active {
  color: var(--active-color);
  border-bottom: 2px solid var(--active-color);
}
</style>
