<script setup>
import Header from '../components/Header.vue'
import Sidebar from '../components/Sidebar.vue'
import UserPost from '../components/UserPost.vue'
</script>
<template>
  <!-- Header Section -->
  <Header />

  <!-- Main Section -->
  <div class="middle py-4 lg:py-7">
   <div class="container mx-auto">
    <div class="grid grid-cols-1 lg:grid-cols-3 gap-12">
    
        <!-- Posts Section -->
        <div class="lg:col-span-2 space-y-4">
        
        
         <div class="flex items-center justify-center mb-12">
              <!-- Card Container -->
              <div class="w-full max-w-4xl rounded-lg overflow-hidden relative">
                <!-- Background Image Section -->
                <div class="relative">
                  <img src="../../assets/img/post-img1.png" alt="Profile background" class="w-full object-cover rounded-2xl">
                </div>
                
              
                
                <!-- Action Buttons Section -->
                <div class="flex justify-between items-start">
                
                  <div class="flex items-center space-x-4 lg:space-x-6 pt-4">
                    <!-- Image icon -->
                    <div class="flex items-center gap-2 lg:gap-3">
                      <img class="w-4 lg:w-6 dark:invert" src="../../assets/img/pic-icon.png" alt=""><span class="text-black dark:text-white font-bold text-xs lg:text-base">225</span>
                    </div>
                    <div class="flex items-center gap-2 lg:gap-3">
                      <img class="w-4 lg:w-6 dark:invert" src="../../assets/img/heart-icon.png" alt=""><span class="text-black dark:text-white text-xs lg:text-base font-bold">225</span>
                    </div>
                  </div>
                  
                  <!-- Profile Information Section -->
                    <div class="text-center mt-8 z-20">
                    <div class="mt-[-80px] lg:mt-[-100px]">
                        <img class="w-20 h-20 lg:w-32 lg:h-32 rounded-full mx-auto object-cover" src="../../assets/img/profile-img2.png" alt="Profile Image">
                      </div>
                      <h2 class="text-sm lg:text-xl 2xl:text-2xl font-bold text-black dark:text-white pt-4">Annie Geturgun</h2>
                      <p class="text-black dark:text-white font-bold pt-2 lg:pt-4 text-xs lg:text-base xl:text-lg 2xl:text-xl">Add Headline</p>
                      <a href="#" class="text-black dark:text-white font-bold pt-1 block text-xs lg:text-base xl:text-lg 2xl:text-xl">echolive.io/anniegeturgun</a>
                    </div>
                    
                    <div class="flex pt-4 w-28 lg:w-auto justify-end">
                  
                      <!-- Share icon -->
                      <div class="flex space-x-4 lg:space-x-6">
                        <a href="#"><img class="w-4 lg:w-6 dark:invert" src="../../assets/img/heart-icon.png" alt=""></a>
                        <a href="#"><img class="w-4 lg:w-6 dark:invert" src="../../assets/img/share-icon.png" alt=""></a>
                      </div>
                  
                  
                  </div>
                  
                  
                </div>
              </div>
            </div>

            <UserPost 
            title="Annie Geturgun" 
            user_id="@honeypie"
            post_date="September 20, 2024"
            description="Here I am at the pool looking very blue" 
            :isLocked="false"
            :isUserPost="false"
            user_image="../../assets/img/post-img1.png"
            />

            <UserPost 
            title="Annie Geturgun" 
            user_id="@honeypie"
            post_date="September 20, 2024"
            description="Here I am at the pool looking very blue" 
            :isLocked="false"
            :isUserPost="true"
            user_image="../../assets/img/post-img2.png"
            />

            <UserPost 
            title="Annie Geturgun" 
            user_id="@honeypie"
            post_date="September 20, 2024"
            description="Here I am at the pool looking very blue" 
            :isLocked="true"
            :isUserPost="false"
            user_image="../../assets/img/post-blur-img1.png"
            />
            

        </div>

        <!-- Sidebar Section -->
        
           <Sidebar />
    </div>
   </div>
  </div>

</template>

<script>
export default {
  components: {
    UserPost,
  },
  data() {
    return {
      
    };
  },
};
</script>