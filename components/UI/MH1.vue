<template>
  <h1
    class="text-4xl sm:text-5xl font-bold leading-none tracking-wider"
    v-text="text"
  />
</template>

<script>
export default {
  props: ['text']
};
</script>
