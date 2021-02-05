<template>
  <div id="app">@{{ user.username }} - {{}}</div>
</template>

<script>
// import Header from "./components/Header";
export default {
  el: "#app",
  name: "App",
  components: {},
  data() {
    return {
      followers: 0,
      user: {
        id: 1,
        username: "_JohnSmith",
        firstName: "John",
        lastName: "Smith",
        email: "johnsmith@xmail.com",
        isAdmin: true,
      },
    };
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
