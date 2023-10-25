<script setup lang="ts">
  import HomeIntroduction from "@/components/molecules/home/HomeIntroduction.vue";
  import HomeSetting from "@/components/molecules/home/HomeSetting.vue";
</script>

<template>
  <div class="container">
    <HomeIntroduction />
    <HomeSetting />
  </div>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
