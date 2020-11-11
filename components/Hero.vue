<template>
  <section class="section ">
    <div class="container sm:mx-12 ">
      <div class="text my-48 ">
        <h1 class="sm:text-2xl font-bold " id="product">Product Design</h1>
        <p class="lorem py-8 font-bold text-4xl">
          Rebranding group <br /> & startup ideas
        </p>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  name: 'Hero'
}
</script>
<style scoped>

h1 {
  font-size: 8.5rem;
  background: -webkit-linear-gradient(
    96.76deg,
    #4158d0 23.44%,
    #c850c0 56.25%,
    #ffcc70 89.05%
  );
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}
@media (max-width: 755px) {
  h1 {
    font-size: 3.5rem;
    background: -webkit-linear-gradient(
      96.76deg,
      #4158d0 23.44%,
      #c850c0 56.25%,
      #ffcc70 89.05%
    );
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
  }
}
</style>
