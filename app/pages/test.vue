<script setup>
const { data } = await useAsyncData(() => queryCollection('content').path('/test').first())
</script>

<template>
  <div>
    <ContentRenderer v-if="data" :value="data" />
  </div>
</template>