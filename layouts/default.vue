<template>
    <div class="w-full">
        <Header/>
    </div>
    <div class="w-full border-y-2 border-gray-300">
        <Header-bottom/>
    </div>
   <div class="bg-white">
        <slot/>
   </div>
    <div class="w-full bg-[#EFF2F4]">
        <Footer-top/>
    </div>
    <div class="w-full bg-white">
        <Footer-middle/>
    </div>
    <div class="w-full bg-[#EFF2F4]">
        <Footer-bottom/>
    </div>
</template>

<script setup>

</script>

<style scoped>

</style>