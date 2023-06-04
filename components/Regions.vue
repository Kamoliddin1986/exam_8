<template lang="">
    <div class="mt-[30px] pb-[45px]">
        <div>
            <h3 class="text-[24px] font-[600]">Suppliers by region</h3>
        </div>
        <div class="grid grid-cols-5 mt-[24px]">
            <div v-for="el in regions1" class="flex w-[221px] h-[36px]  items-center">
                <div class="w-[28px] h-[20px]">
                    <img :src="el.flag" alt="" class="w-[28px] h-[20px]">
                </div>
            
                <div class="w-[190px] h-[36px] ml-[10px]">
                    <h4 class="text-[16px] font-[400] ">{{el.country}}</h4>
                    <p class="text-[13px] text-[#8B96A5]">{{el.site}}</p>
                </div>
            </div>
        </div>
        <div class="grid grid-cols-5 mt-[20px]">
            <div v-for="el2 in regions2" class="flex w-[221px] h-[36px]  items-center">
                <div class="w-[28px] h-[20px]">
                    <img :src="el2.flag" alt="" class="w-[28px] h-[20px]">
                </div>
            
                <div class="w-[190px] h-[36px] ml-[10px]">
                    <h4 class="text-[16px] font-[400] ">{{el2.country}}</h4>
                    <p class="text-[13px] text-[#8B96A5]">{{el2.site}}</p>
                </div>
            </div>

        </div>

    </div>
</template>
<script setup>

</script>
<style lang="">
    
</style>