<script setup lang="ts">
defineProps<{
  testProp?: string
}>()
</script>

<template>
  <div>
    <h1>Test component</h1>
    <slot name="title" />
    <h1>Test component end</h1>
    <img v-if="testProp" :src="testProp" />
  </div>
</template>