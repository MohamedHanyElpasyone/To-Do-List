<script setup lang="ts">
import { MoonIcon, SunIcon } from '@heroicons/vue/24/outline';
import { ref } from 'vue';

const isDark = ref(false);

const themeToggler = () => {
    isDark.value = !isDark.value;
    if (isDark.value) {
        document.documentElement.classList.add('dark')
        localStorage.setItem('theme', 'dark')
    }
    else {
        document.documentElement.classList.remove('dark')
        localStorage.setItem('theme', 'light')
    }
}
function checkTheme() {
    const theme = localStorage.getItem('theme')
    if (theme === 'dark') {
        isDark.value = true
        document.documentElement.classList.add('dark')
    }
    else {
        isDark.value = false
        document.documentElement.classList.remove('dark')
    }
}
checkTheme()
</script>

<template>
    <!-- CONTAINER -->
    <div class="flex justify-end">
    <button class="w-12 mr-10 mt-7 cursor-pointer" @click="themeToggler()">
        <MoonIcon v-if="!isDark" />
        <SunIcon v-else class="text-white" />
    </button>
    </div>
</template>
