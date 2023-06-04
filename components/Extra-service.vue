<template lang="">
    <div class="mt-[30px] w-[100%]">
        <div>
            <h3 class="text-[24px] font-[600]">
                Our extra services
            </h3>
        </div>

        <div class="grid grid-cols-4 gap-[20px]">
            <div v-for="el in extra_service" class="card w-[100%] h-[200px] relative border border-grey-400 rounded-[10px] bg-white mt-[24px] h-[200px]">
                <div class="rounded-t-[10px] w-[100%] h-[120px] bg-black" >
                    <img :src="el.image" alt="" class="opacity-70 w-[100%] h-[120px] rounded-t-[10px]">
                </div>
                <div class="w-[55px] h-[55px] bg-[#D1E7FF] border absolute border-white border-2 rounded-full left-[220px] bottom-[49px] flex items-center justify-center">
                    <Icon :name="el.icon" color="#1C1C1C" class="text-[24px]" />
                </div>
                <div class="h-[44px] w-[160px] mt-[16px] mb-[20px] ml-[20px] ">
                    <p class="text-[16px] font-[500] text-[#1C1C1C]">
                        {{el.text}}
                    </p>
                </div>

                
            </div>
        </div>
    </div>
</template>
<script setup>

</script>
<style lang="">
    
</style>