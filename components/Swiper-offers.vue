<template>
    <Swiper
    :modules="[SwiperAutoplay, SwiperNavigation]"
    navigation 
    :autoplay="{
      delay: 4000,
      disableOnInteraction: true,
    }"
    :slides-per-view="5" :space-between="0" :loop="true"
  >
    <SwiperSlide v-for="slide in offers" :key="slide.id">
        <div class="flex flex-col gap-2 px-[38px] py-[17px] justify-center items-center border">
            <img :src="slide.image" class="w-[120px] h-[135px]" alt="">
            <p>{{ slide.name }}</p>
            <p class="bg-[#FFE3E3] px-2 py-[2px] text-[#EB001B] rounded-full">{{ slide.offer }}</p>
        </div>
    </SwiperSlide>
  </Swiper>
</template>

<script setup>

</script>

<style lang="scss" scoped>

</style>