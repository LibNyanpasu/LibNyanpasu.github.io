<script lang="ts" setup>
const isDev = import.meta.env.DEV
</script>

<template>
  <div
    v-if="isDev"
    className="fixed bottom-1 left-1 flex h-6 w-6 items-center justify-center rounded-full bg-gray-800 p-3 font-mono text-xs text-white"
    style="z-index: 2000"
  >
    <div className="block sm:hidden">xs</div>
    <div className="hidden sm:block md:hidden lg:hidden xl:hidden 2xl:hidden">
      sm
    </div>
    <div className="hidden md:block lg:hidden xl:hidden 2xl:hidden">md</div>
    <div className="hidden lg:block xl:hidden 2xl:hidden">lg</div>
    <div className="hidden xl:block 2xl:hidden">xl</div>
    <div className="hidden 2xl:block">2xl</div>
  </div>
</template>
