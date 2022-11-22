<template>
  <div class="footer">
    <span>Inspired&nbsp;by&nbsp;<NuxtLink :to="link" target="_blank">Notion</NuxtLink></span>
  </div>
</template>

<script setup>
const year = (new Date).getFullYear()
const link = 'https://www.notion.so/product'
</script>

<style scoped>
.footer {
  border-top: 1px solid var(--border-color);

  padding: 1rem 0;
}

</style>
