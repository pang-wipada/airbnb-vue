<template>
  <div>
    <h1>Contact</h1>
    <h2>{{ address }}</h2>
    <UserProfile></UserProfile>
    <hello-world msg="Hello 1"></hello-world>
    <hello-world msg="Hello 2"></hello-world>
    <hello-world></hello-world>
    <hello-world></hello-world>
  </div>
</template>

<script>
import HelloWorld from "@/components/HelloWorld.vue";
import UserProfile from "@/components/UserProfile.vue";

export default {
  data() {
    return {
      address: "Prince of Songkla University, Phuket"
    };
  },
  components: {
    HelloWorld,
    UserProfile
  }
};
</script>

<style>
</style>