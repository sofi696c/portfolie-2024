
<template>
    <div class="carousel">
        <slot></slot>

    <!--   <button @click="next" class="next carousel-knap">Next</button>
      <button @Click="prev" class="prev carousel-knap">Prev</button>
 -->
    </div>
  </template>

<script>
  export default {
    data() {
      return {

      }
    },
    methods: {
      next() {
        this.$emit('next');
      },
      prev() {
        this.$emit('prev');
      }
    }
  }
</script>



<style>
  .carousel {
    position: relative;
    height: 500px;
    width: 70%;
    overflow: hidden;
    margin-top: 20%;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1); /* Add box-shadow for depth */
  }

  .carousel-knap {
    height: 40px;
    width: 50px;
    top: calc(50% - 20px);
  }

  button:focus, button:hover {
    outline: none;
    cursor: pointer;
  }

  .next {
    right: 0;
  }

  .prev {
    left: 0;
  }

</style>