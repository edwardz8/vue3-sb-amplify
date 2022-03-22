<template>
  <div v-editable="blok">
    <div :key="blok._uid" v-for="blok in blok.columns">
      <StoryblokComponent :blok="blok" />
    </div>
  </div>
</template>

<script setup>
defineProps({ blok: Object });
</script>
