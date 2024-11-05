<template>
    <div class="bg-white rounded-lg shadow-md overflow-hidden">
        <div class="relative">
            <img src="../../assets/img/profile-block-post-img.png" alt="Profile image" class="w-full h-28 sm:h-40 md:h-52 object-cover object-bottom">
            <div class="absolute inset-0 bg-gradient-to-t from-black opacity-50"></div>
            <div class="absolute bottom-0 left-0 p-2 lg:p-3 flex items-center justify-between w-full bg-gradient-to-t from-[#825405] to-[#f6dd7b] dark:bg-gradient-to-b">
                <div class="flex items-center">
                <img src="../../assets/img/profile-img1.png" alt="Avatar" class="w-9 h-9 lg:w-16 lg:h-16 2xl:w-20 2xl:h-20 rounded-full mt-[-50px] lg:mt-[-80px]">
                <div class="ml-1 lg:ml-3 2xl:ml-4 text-white">
                    <h2 class="font-bold text-xs lg:text-lg 2xl:text-xl">Honey Pie</h2>
                    <p class="text-[9px] lg:text-sm 2xl:text-base font-semibold">@honeypie</p>
                </div>
                </div>
                <div class="toggle-dropdown"><a href="#"><img class="h-5 2xl:h-7" src="../../assets/img/toggle-dot.png" alt=""></a></div>
            </div>
        </div>
    </div>
</template>