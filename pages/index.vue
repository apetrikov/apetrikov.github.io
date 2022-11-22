<!--App has only one layout here-->
<template>
  <div class="page">
    <Header />
    <div class="content">
    </div>
    <Footer />
  </div>
</template>
<script lang="ts" setup>

</script>
<style>
.page {
  display: flex;
  flex-direction: column;

  min-height: 100vh;
}

.content {
  flex: 1;
}
</style>