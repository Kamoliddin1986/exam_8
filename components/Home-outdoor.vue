<template lang="">
    <div class="flex grid-col-2 border border-grey-400 h-[257px]  mt-[23px] rounded-[10px]">
        <div class="w-[25%] h-[257px] rounded-l-[10px] bg-cover" style="background-image: url(fon.png)">
            <div class="w-[130px] h-[52px]">
                <h1 class="text-[20px] font-semibold text-[#1C1C1C] mt-[20px] ml-[20px]"> Home and outdoor</h1>

            </div>
            <button class="bg-white rounded-[10px] ml-[20px] w-[132px] h-[40px] text-[16px] font-medium mt-[16px]"> Source now</button>
        </div>
        <div class="w-[75%] h-[257px]">
            <div class="">
                <div  class="grid grid-cols-4 ">
                    <div v-for="el in home_outdoor1" class=" flex border border-grey-400  h-[128px] bg-white">
                        <div class="pl-[16px] pt-[20px]">
                            <h3 class="text-[16px] font-normal"> {{el.title}}</h3>
                            <p class="text-[13px] text-[#8B96A5]">From</p>
                            <p class="text-[13px] text-[#8B96A5]">USD {{el.price}}</p>
                        </div>
                        <div class=" flex items-end w-[62px] h-[62px] mt-[42px] ml-[50px] p-[8px]">
                            <img :src='el.image' alt="">
                        </div>
                    </div>
                    
                </div>
                <div class="grid grid-cols-4">
                    <div v-for="el2 in home_outdoor2" class=" flex border border-grey-400  h-[128px] bg-white">
                        <div class="pl-[16px] pt-[20px]">
                            <h3 class="text-[16px] font-normal"> {{el2.title}}</h3>
                            <p class="text-[13px] text-[#8B96A5]">From</p>
                            <p class="text-[13px] text-[#8B96A5]">USD {{el2.price}}</p>
                        </div>
                        <div class=" flex items-end w-[62px] h-[62px] mt-[42px] ml-[50px] p-[8px]">
                            <img :src="el2.image" alt="">
                        </div>
                    </div>
                    
                </div>
            </div>
            
        </div>
    </div>
</template>
<script setup>

</script>
<style lang="">
  
</style>