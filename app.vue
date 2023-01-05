<template>
  <div>Hello World!</div>
  <button @click="increment">+</button>
  <p>{{ count }}</p>
  <button @click="decrement">-</button>
  <p>
    Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusamus
    sit porro neque quis vero voluptatibus sequi nisi id ullam iure,
    rerum velit, nihil dolores doloribus ab totam voluptas optio
    voluptatum!
  </p>
</template>

<script setup>
//  Composition API
const count = ref(0);
function increment() {
  count.value++;
}
function decrement() {
  count.value--;
}
</script>
<!-- <script>
// Optoins API
export default {
  data() {
    return {
      count: 0,
    };
  },
  methods: {
    increment() {
      this.count++;
    },
    decrement() {
      this.count--;
    },
  },
};
</script> -->
