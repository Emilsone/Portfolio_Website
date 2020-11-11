<template>
  <section class="text-gray-700 body-font">
    <div
      class="container mx-auto flex px-5 py-24 md:flex-row flex-col items-center"
    >
      <div
        class="lg:flex-grow md:w-1/2 lg:pr-24 md:pr-16 flex flex-col md:items-start md:text-left mb-16 md:mb-0 items-center text-center"
      >
        <h1
          class="title-font sm:text-4xl text-3xl mb-4 font-medium text-gray-900"
        >
          I’m James Moses
        </h1>
        <p class="mb-8 leading-relaxed text-2xl">
          My passion is designing products and services that delight users and
          make their lives better, easier or more beautiful.
        </p>
        <div class="flex justify-center">
          
          <button
            class="ml-4 inline-flex text-black bg-white border-0 py-2 px-6 focus:outline-none hover:bg-gray-300 rounded text-lg"
          >
            Hire James 
          </button>
        </div>
      </div>
      <div class="lg:max-w-lg lg:w-full md:w-1/2 w-5/6">
        <img
          class="object-cover object-center rounded"
          alt="hero"
          src="~/assets/img/about-james.png"
        />
      </div>
    </div>
  </section>
</template>
<script>
export default {
  name: "about",
};
</script>

