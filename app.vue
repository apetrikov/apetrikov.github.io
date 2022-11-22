<!--App has only one layout here-->
<template>
    <NuxtPage />
</template>

<script setup lang="ts">
</script>

<style>
@import 'assets/styles/variables.css';

@media (prefers-color-scheme: dark) {
  html {
    --background: var(--dm-background);
    --text: var(--dm-text);
    --text-medium: var(--dm-text-medium);
    --border-color: var(--dm-border-color);
  }
}

@media (prefers-color-scheme: light) {
  html {
    --background: var(--lm-background);
    --text: var(--lm-text);
    --text-medium: var(--lm-text-medium);
    --border-color: var(--lm-border-color);
  }
}

body {
  transition: background 0.2s ease;

  margin: 0 2rem;
  font-family: inter-var, -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, "Apple Color Emoji", Arial, sans-serif, "Segoe UI Emoji", "Segoe UI Symbol",serif;
  background: var(--background);
  color: var(--text-medium);
}

h1, h2, h3, h4, h3, h5, h6 {
  color: var(--text);
}

a {
  color: var(--link);

  text-decoration: underline;
  text-underline-offset: 0.1em;
  text-decoration-thickness: 1px;
}

a:hover {
  color: var(--link-hover);
  text-decoration: none;
}

a:active {
  color: var(--link-active);
  text-decoration: none;
}

a:visited {
  color: var(--link);
}
</style>