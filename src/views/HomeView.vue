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
            <!-- Post 1 -->
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
