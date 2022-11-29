<template>
  <a @click="toggleDark()" cursor-pointer>
    <div i-carbon-sun v-show="!isDark" />
    <div i-carbon-moon v-show="isDark" />
  </a>
</template>

<script setup lang="ts">
  import { isDark } from '~/utils';
  import { useToggle } from '@vueuse/core';

  const toggleDark = useToggle(isDark);
</script>
