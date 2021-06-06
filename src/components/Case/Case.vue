<template>
  <div class="case">
    <div class="container">
      <div class="case__title">Кейсы:</div>
      <div class="case__wrapper">
        <Cases :content="text" />
        <Cases :content="text" />
        <Cases :content="text" />
        <Cases :content="text" />
        <Cases :content="text" />
        <Cases :content="text" />
        <Cases :content="text" />
        <Cases :content="text" />
        <Cases :content="text" />
        <Cases :content="text" />
        <Cases :content="text" />
        <Cases :content="text" />
        <Cases :content="text" />
        <Cases :content="text" />
        <Cases :content="text" />
        <Cases :content="text" />
        <Cases :content="text" />
        <Cases :content="text" />
        <Cases :content="text" />
        <Cases :content="text" />
      </div>
      <div class="case__footer">
        <Cases :content="text" />
        <Cases class="case__last" :content="text" />
      </div>
    </div>
  </div>
</template>

<script>
import Cases from "@/components/Elements/Cases/Cases";
export default {
  name: "Case",
  components: {Cases},
  data() {
    return {
      text: {
        title: "WOG Pride",
        subtitle: "Приложение для сети автозаправочных комплексов WOG"
      }
    }
  }
}
</script>

<style lang="scss">
@import "case";
</style>