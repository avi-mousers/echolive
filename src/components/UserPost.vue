<script setup>
import UserSubPost from './UserSubPost.vue'
import SharePost from './SharePost.vue'
</script>
<template>
    
        <!-- Post 2 -->
        <div class="bg-white dark:bg-gradient-to-tl dark:from-[#825405] dark:to-[#f6dd7b] rounded-lg">
            <div class="flex justify-between items-center mb-2 p-4 xl:p-6 2xl:p-9 pt-2 pb-2 xl:pt-4 xl:pb-4 2xl:pt-6 2xl:pb-6">

            <div class="flex items-center space-x-4">
                <div class="w-9 h-9 lg:w-16 lg:h-16 2xl:w-20 2xl:h-20 bg-gray-700 rounded-full"><img src="../../assets/img/profile-img2.png" alt=""></div>
                <div>
                    <div class="text-black font-bold text-xs lg:text-base xl:text-xl 2xl:text-2xl">{{title}}</div>
                    <span class="text-yellow-900 dark:text-black text-[9px] xl:text-sm xl:text-base 2xl:text-lg font-semibold block">{{user_id}}</span>
                </div>
            </div>

            <div class="flex">
                <div class="flex items-center space-x-2">
                    <span class="text-[9px] lg:text-base xl:text-xl 2xl:text-2xl text-black font-semibold pr-2 lg:pr-4">{{post_date}}</span>
                </div>
                <div class="text-black font-bold text-xs lg:text-base xl:text-xl 2xl:text-2xl">•••</div>
            </div>
            
        </div>
        
        <div class="text-black font-semibold  text-xs lg:text-base xl:text-lg 2xl:text-xl p-4 xl:p-6 2xl:p-9 xl:pb-4 pt-0 xl:pt-0">
        <p>{{description}}</p>
        </div>


        <div v-if="!isLocked" class="mb-0"><img :src="user_image" alt=""></div>

        <div v-if="isLocked" class="mb-0">
            <div class="w-full  bg-gray-300 relative">
            <img :src="user_image" alt="">
                <div class="absolute inset-0 backdrop-blur-lg bg-opacity-70"></div>
                <!-- Lock Icon -->
                <div class="absolute inset-0 flex flex-col items-center justify-center text-center">
                    <div class="p-3 md:p-4">
                        <img class="h-16 lg:h-28 2xl:h-auto" src="../../assets/img/lock-icon.png" alt="">
                    </div>
                    <div class="mt-2 lg:mt-4 text-center">
                        <button class="bg-gradient-to-b from-[#f1dc82] to-[#865909] dark:bg-gradient-to-b dark:from-black dark:to-black text-white  text-xs md:text-sm lg:text-base font-bold py-2 px-4 lg:py-3 md:px-6 rounded-full shadow-lg">
                            Subscribe to Unlock
                        </button>
                    </div>
                </div>
            </div>        
        </div>
        
        <SharePost />
        
        <div v-if="isUserPost" class="grid grid-cols-2 gap-4 lg:gap-6 2xl:gap-8 p-4 pb-4 lg:p-6 lg:pb-6 pt-0 lg:pt-0 2xl:pt-0 2xl:p-9 2xl:pb-9">
            <!-- Card 1 -->
            <UserSubPost />
            <!-- Card 2 -->
            <UserSubPost />
            
        </div>
        
    </div>

    
   
</template>


<script>
export default {
  props: {
    title: {
      type: String
    },
    user_id: {
      type: String,
    },
    description: {
      type: String,
      default: 'No description provided.',
    },
    post_date: {
      type: String,
    },
    isUserPost: {
      type: Boolean,
      default: false
    },
    isLocked: {
      type: Boolean,
      default: false
    },
    user_image: {
      type: String,
    }
  },
};
</script>