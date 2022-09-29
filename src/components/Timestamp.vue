<template>
  <span className="timestamp">{{ timestamp }}</span>
</template>

<script setup>
defineProps({
  timestamp: {
    type: String,
  },
});
</script>
