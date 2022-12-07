<template>
  <div class="tweet">
    <ProfileImage :image="tweet.user.image" />
    <div class="body">
    <div class="top">
      <User :usuario="tweet.user" />
        <Timestamp :tiempo="tweet.timestamp" />
     </div>
          
    <Message :mensaje="tweet.message" />
    <Actions/>
    
  </div>
  <i class="fas fa-ellipsis-h"></i>
    
  </div>

</template>

<script>
import User from "./User.vue";
import Timestamp from "./Timestamp.vue";
import Message from "./Message.vue";
import ProfileImage from "./ProfileImage.vue";
import Actions from "./Actions.vue";

export default {
  components: {
    User,
    Timestamp,
    Message,
    ProfileImage,
    Actions,
  },
  props: ["tweet"],
};
</script>
<style scoped>
a {
  color: #42b983;
}
</style>
