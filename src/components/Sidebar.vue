<script setup>
import SidebarPost from './SidebarPost.vue'
</script>
<template>
    <div class="space-y-10">
        <!-- Subscription Card -->
        <div class="bg-white dark:bg-gradient-to-b dark:from-[#825405] dark:to-[#f6dd7b] text-black  dark:text-white p-4 rounded-lg text-center ">
            <h2 class="text-xs lg:text-base xl:text-xl 2xl:text-2xl font-bold">SUBSCRIPTION</h2>
            <p class="text-xs lg:text-sm 2xl:text-base font-semibold pt-1 pb-1">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut blandit nisl eu.</p>
            <button class="bg-gradient-to-b from-[#f1dc82] to-[#865909] text-white shadow-lg dark:bg-gradient-to-b dark:from-black dark:to-black  text-white text-xs md:text-sm lg:text-base font-bold py-2 px-4 lg:py-3 md:px-6 rounded-full mt-2">Subscribe for FREE</button>
        </div>
        <SidebarPost />
        <SidebarPost />
        <SidebarPost />        
    </div>
</template>