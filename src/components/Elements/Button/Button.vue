<template>
    <a class="btn" :style="`background-color: ${content.color}`" href="#"><span>{{ content.text }}</span></a>
</template>

<script>
export default {
  props: ["content"],
  name: "Button",
}
</script>

<style lang="scss">
@import "button";
</style>