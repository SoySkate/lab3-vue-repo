<template>
  <p className="message">
    {{ message }}
  </p>
</template>

<script setup>
defineProps({
  message: {
    type: String,
  },
});
</script>
