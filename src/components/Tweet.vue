<template>
  <div className="tweet">
    <ProfileImage :profileImage="user.image" />

    <div className="body">
      <div className="top">
        <User :user="user" />
        <Timestamp :timestamp="timestamp" />
      </div>

      <Message :message="message" />

      <Actions />
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>

<style scoped>
a {
  color: #42b983;
}
</style>

<script setup>
import Actions from "./Actions.vue";
import Message from "./Message.vue";
import Timestamp from "./Timestamp.vue";
import User from "./User.vue";
import ProfileImage from "./ProfileImage.vue";
defineProps({
  message: {
    type: String,
  },
  timestamp: {
    type: String,
  },
  user: {
    type: Object,
  },
  profileImage: {
    type: String,
  },
});
</script>
