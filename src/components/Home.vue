<template>
  <h1>Hi, Welcome On Home Page</h1>
</template>
<script>
export default {
  name: "Home",
  mounted() {
    let user = localStorage.getItem("user-info");
    if (!user) {
      this.$router.push({ name: "SignUp" });
    }
  },
};
</script>
<style></style>
