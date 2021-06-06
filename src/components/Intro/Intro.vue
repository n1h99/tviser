<template>
  <div class="intro">
    <div class="container">
      <div class="intro__inner">
        <div class="intro__left">
          <div class="intro__title">{{ title }}</div>
          <svg width="140" height="16" viewBox="0 0 140 16" fill="none" xmlns="http://www.w3.org/2000/svg">
            <g filter="url(#filter0_dd)">
              <path d="M4 4L136 4" stroke="black" stroke-width="8"/>
            </g>
            <defs>
              <filter id="filter0_dd" x="0" y="0" width="140" height="16" filterUnits="userSpaceOnUse" color-interpolation-filters="sRGB">
                <feFlood flood-opacity="0" result="BackgroundImageFix"/>
                <feColorMatrix in="SourceAlpha" type="matrix" values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"/>
                <feOffset dy="4"/>
                <feGaussianBlur stdDeviation="2"/>
                <feColorMatrix type="matrix" values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.25 0"/>
                <feBlend mode="normal" in2="BackgroundImageFix" result="effect1_dropShadow"/>
                <feColorMatrix in="SourceAlpha" type="matrix" values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"/>
                <feOffset dy="4"/>
                <feGaussianBlur stdDeviation="2"/>
                <feColorMatrix type="matrix" values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.25 0"/>
                <feBlend mode="normal" in2="effect1_dropShadow" result="effect2_dropShadow"/>
                <feBlend mode="normal" in="SourceGraphic" in2="effect2_dropShadow" result="shape"/>
              </filter>
            </defs>
          </svg>
          <div class="intro__subtitle">{{ subtitle }}</div>
          <Button class="intro__btn" :content="btn"/>
        </div>
        <div class="intro__right">
          <Img src="/images/intro/intro_img.png" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Button from "@/components/Elements/Button/Button";
export default {
  props: ["content"],
  name: "Intro",
  components: {Button},
  data() {
    return {
      title: 'Разработка мобильных приложений для бизнеса',
      subtitle: 'Мобильная разработка, заточенная под удобство конечного пользователя',
      btn: {
        text:"Рассчитать проект",
        color:"#000000"
      }
    }
  }
}
</script>

<style lang="scss">
@import "intro";
</style>