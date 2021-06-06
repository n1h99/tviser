<template>
  <div class="task">
    <div class="container">
      <div class="task__inner">
        <div class="task__title">{{ title }}</div>
        <div class="task__subtitle">Дайте новую жизнь своему проекту.<br> Нажмите Заказать и мы бесплатно просчитаем стоимость</div>
        <Button class="task__btn" :content="btn" />
      </div>
    </div>
  </div>
</template>

<script>
import Button from "@/components/Elements/Button/Button";
export default {
  name: "Task",
  components: {Button},
  data() {
    return {
      title:"Определяем и решаем бизнес-задачи клиентов.",
      btn: {
        text: "Рассчитать проект",
        color:"#000000"
      }
    }
  }
}
</script>

<style lang="scss">
@import "task";
</style>