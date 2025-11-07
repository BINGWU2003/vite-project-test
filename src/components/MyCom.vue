<template>
  <div>
    <h1>My Component</h1>
    <h2>{{ name }}</h2>
    <button @click="handleClick">Click me</button>
  </div>
</template>

<script setup lang="ts">
const props = defineProps<{
  name: string;
}>();

console.log(props.name);

const handleClick = () => {
  console.log('Button clicked');
};
</script>

<style lang="scss" scoped>
h1 {
  color: red;
}
</style>
