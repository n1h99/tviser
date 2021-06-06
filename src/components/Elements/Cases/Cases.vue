<template>
 <div class="cases">
   <Img src="/images/cases/cases_logo.png"/>
   <div class="cases__title"><span>{{ content.title }}</span></div>
   <div class="cases__text"><span>{{ content.subtitle }}</span></div>
 </div>
</template>

<script>
export default {
  props:["content"],
  name: "Cases"
}
</script>

<style lang="scss">
@import "cases";
</style>