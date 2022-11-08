<!--App has only one layout here-->
<template>
  <Html :class="classObject">
    <Header/>
    <button @click="toggleTheme">Toggle</button>
  </Html>
</template>
<script lang="ts" setup>
  const isLightTheme = ref<boolean>(true)

  const toggleTheme = (): void => isLightTheme.value = !isLightTheme.value

  const classObject = computed(() => ({
    'lightTheme': isLightTheme.value,
    'darkTheme': !isLightTheme.value
  }))
</script>
<style>
@import 'assets/styles/global.css';

html.lightTheme, body.lightTheme {
  --background: var(--lm-background);
  --text: var(--lm-text);
  --text-medium: var(--lm-text-medium);
}

html.darkTheme, body.darkTheme {
  --background: var(--dm-background);
  --text: var(--dm-text);
  --text-medium: var(--dm-text-medium);
}

html, body {
  background: var(--background);
  color: var(--text);
}

</style>