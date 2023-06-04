<template lang="">
    <div class=" w-[100%]  mt-[30px]">
        <div>
            <h1 class="text-[24px] font-[600] ">
                Recomended items
            </h1>
        </div>

        <div class="grid grid-cols-5 gap-[25px] h-[310px] w-[100%] mt-[24px]">
            <div v-for="el in recomended1" class="card w-[235px] h-[310px] border border-grey-400 rounded-[5px] bg-white">
                <div class="w-[190px] h-[200px] mt-[14px] ml-[24px] mb-[15px] flex align-center justify-center">

                    <img :src="el.image" alt="" >
                </div>
                <div class="pl-[16px]">
                    <h3 class="text-[16px] font-[500]">
                        {{el.price}}
                    </h3>
                    <div class="w-[186px] h-[53px]">
                        <p class="font-[400] text-[16px] text-[#8B96A5]">{{el.title}}</p>

                    </div>
                    
                </div>
            </div>
        </div>

        <div class="grid grid-cols-5 gap-[25px] h-[310px] w-[100%] mt-[24px]">   
            <div v-for="el2 in recomended2" class="w-[235px] h-[310px] border border-grey-400 rounded-[5px] bg-white">
                <div class="w-[190px] h-[200px] mt-[14px] ml-[24px] mb-[15px] flex align-center justify-center">

                    <img :src="el2.image" alt="" >
                </div>
                <div class="pl-[16px]">
                    <h3 class="text-[16px] font-[500]">
                        {{el2.price}}
                    </h3>
                    <div class="w-[186px] h-[53px]">
                        <p class="font-[400] text-[16px] text-[#8B96A5]">{{el2.title}}</p>

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