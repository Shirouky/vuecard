<template>
  <div id="app">
    <UserCard
      :username="username"
      :name="name"
      :surname="surname"
      :location="location"
      :mail="mail"
      :phone="phone"
    />
  </div>
</template>

<script>
import UserCard from "./components/UserCard.vue";

export default {
  name: "App",
  components: {
    UserCard,
  },
  data() {
    return {
      username: "romashka",
      name: "Иван",
      surname: "Иванов",
      location: "Москва, Юбилейная 50",
      mail: "coldrabbit48@example.com",
      phone: "+7-495-266-57-34",
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
  margin-top: 60px;
}
</style>
