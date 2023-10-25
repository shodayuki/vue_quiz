<script setup lang="ts">
  import { useCategories } from "@/composables/categories";

  const { categories, checkbox, checkAll, checkAllOff, goQuiz } = useCategories()
</script>

<template>
  <section class="home-quiz__setting">
    <h2 class="home-quiz__setting-h2">出題設定</h2>
    <form>
      <label v-for="(category, index) in categories" :key="index">
        <input type="checkbox" v-model="checkbox" :value="category.id" checked />
        {{ category.name }}&ensp;
      </label>
      <div>
        全項目チェック
        <button type="button" @click="checkAll">ON</button>
        <button type="button" @click="checkAllOff">OFF</button>
      </div>
      <button type="button" class="btn btn-primary" @click="goQuiz">出題開始</button>
    </form>
  </section>
</template>