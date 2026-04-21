<script setup lang="ts">
import ThemeTogglerButton from './components/ThemeTogglerButton.vue'
import AddInput from './components/AddInput.vue'
import TasksList from './components/TasksList.vue'
import { onMounted } from 'vue'
import twemoji from 'twemoji'

onMounted(() => {
  twemoji.parse(document.body, {
    folder: 'svg',
    ext: '.svg',
  })
})
</script>

<template>
  <main>
    <ThemeTogglerButton />
    <section class="flex flex-col items-center mx-48">
      <h1 class="font-bold text-4xl mt-2 text-[#333333] dark:text-white">My Tasks</h1>
      <AddInput />
      <TasksList />
    </section>
  </main>
</template>
