<script setup lang="tsx">
import CommitButton from '../widgets/commit-button.vue';
</script>

<template>
  <div class="w-screen h-screen flex flex-row gap-6 items-center justify-center bg-stone-950">
    <CommitButton badge="📌 start"/>
    <CommitButton badge="🎯 feats"/>
    <CommitButton badge="🛠️ fixes"/>
    <CommitButton badge="🧩 tests"/>
    <CommitButton badge="📘 docs"/>
  </div>
</template>