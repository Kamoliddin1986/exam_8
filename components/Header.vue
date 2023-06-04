<template>

    <div class="container mx-auto px-[130px]">
        <div class="flex h-[86px] py-[20px] items-center justify-between">
            <img src="/logo-colored.svg" alt="">

            <div class="flex h-[40px] ">
                <input type="text" placeholder="Search" class="border border-[#0D6EFD] border-y-2 border-l-2 rounded-l-md focus:outline-none focus:ring-1 focus:ring-[#0D6EFD] w-[420px]">
                <select id="currency" name="currency" class=" border border-[#0D6EFD] border-y-2 border-l-[1px] bg-transparent py-0 pl-2 pr-7  focus-visible:outline-none focus:ring-1 sm:text-sm">
                    <option>All Categories</option>
                    <option>CAD</option>
                    <option>EUR</option>
                </select>
                <button class="bg-[#0D6EFD] text-white px-6 py-2 rounded-r-md">Search</button>
            </div>

            <div class="flex gap-3">
                <div class="flex flex-col items-center justify-center text-gray-500">
                    <Icon name="ic:baseline-person" class="text-[23px] " />
                    <p class="text-[12px]">Profile</p>
                </div>
                <div class="flex flex-col items-center justify-center text-gray-500">
                    <Icon name="material-symbols:chat-rounded" class="text-[23px] " />
                    <p class="text-[12px]">Message</p>
                </div>
                <div class="flex flex-col items-center justify-center text-gray-500">
                    <Icon name="mdi:heart" class="text-[23px] " />
                    <p class="text-[12px]">Orders</p>
                </div>
                <div class="flex flex-col items-center justify-center text-gray-500">
                    <Icon name="ic:sharp-shopping-cart" class="text-[23px] " />
                    <p class="text-[12px]">My Cart</p>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>

</script>

<style scoped>

</style>