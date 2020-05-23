<template>
  <h1>Listing Detail {{ id }}</h1>
</template>

<script>
import axios from "axios";
export default {
  data() {
    return {
      id: this.$route.params.id
    };
  },
  mounted() {
    let url =
      "https://pangairbnbapi.azurewebsites.net/api/airbnb/listings/city/";
    url = url + this.id;
    axios.get(url).then(response => {
      console.log(response.data);
    });
  }
};
</script>

<style>
</style>