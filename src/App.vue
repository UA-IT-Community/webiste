<script setup lang="ts">
import { RouterView } from "vue-router";
import { useDark, useToggle, useTitle } from '@vueuse/core'

const isDark = useDark()
const toggleDark = useToggle(isDark)
useTitle('🇺🇦 IT Спільнота')

</script>

<template>
  <div class="app">
    <div class="app-header">
      <i></i>
      <i></i>
      <i></i>
    </div>

    <div class="app-body">
      <RouterView />
    </div>
    <div class="toggle">
      <input
        type="checkbox"
        id="toggle"
        :checked="isDark"
        @click="(e) => toggleDark()"
      />
      <label for="toggle" />
    </div>
  </div>
</template>
