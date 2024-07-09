<script setup lang="tsx">
const props = defineProps<{
  badge: string
}>();

function copyCommitMessage() {
  const commitMessage = `${props.badge} #${Date.now()}`;

  navigator.clipboard.writeText(commitMessage);
}
</script>

<template>
  <button class="p-4 border rounded-lg border-stone-100 text-stone-100" @click="copyCommitMessage">
    {{ props.badge }}
  </button>
</template>