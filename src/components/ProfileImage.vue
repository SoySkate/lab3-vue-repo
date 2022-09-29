<template>
  <img
    :src="profileImage"
    referrerpolicy="no-referrer"
    className="profile"
    alt="profile"
  />
</template>

<script setup>
defineProps({
  profileImage: {
    type: String,
  },
});
</script>
