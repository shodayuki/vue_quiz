<script setup lang="ts">
  import { useInformations } from "@/composables/informations";
  const { informations } = useInformations()
</script>

<template>
  <section class="home__notice">
    <h2 class="home__notice-h2">お知らせ情報</h2>
    <dl v-for="(info, index) in informations" :key="index">
      <dt>{{ info.created_at }}</dt>
      <dd>{{ info.information }}</dd>
    </dl>
  </section>
</template>