<script>
export default {
  name: "Navbar",
  mounted() {},
  methods: {
    buyTickets: function () {
      alert(
        "The website is under development. Please try again once it is officially published"
      );
    },
    expandBurger: function () {
      // document.getElementById("nav-item").classList.toggle("show"); // Function to expand/collapse the dropdown\

      var elements = document.getElementsByClassName("nav-item");
      for (var i = 0; i < elements.length; i++) {
        elements[i].classList.toggle("show");
      }
    },
  },
};
</script>
<template>
  <div class="navbar">
    <div class="navbar-container">
      <div style="align-items: center" class="heading-container">
        <i class="fa fa-search search-icon"></i>
        <div class="heading">Софийски музеи</div>
        <div class="button-container">
          <button v-on:click="buyTickets()" class="button">Билети</button>
        </div>
      </div>
      <hr />
      <ul class="nav-items">
        <i
          v-on:click="expandBurger()"
          id="bars-icon"
          style="color: white"
          class="fa fa-bars bars-icon"
        ></i>
        <li class="nav-item">
          <router-link to="/"> Начало </router-link>
        </li>
        <li class="nav-item">
          <router-link to="/музеи"> Музеи </router-link>
        </li>
        <li class="nav-item">
          <router-link to="/събития"> Събития </router-link>
        </li>
        <li class="nav-item">
          <router-link to="/галерия"> Галерия </router-link>
        </li>
        <li class="nav-item">
          <router-link to="/контакти"> Контакти </router-link>
        </li>
      </ul>
    </div>
  </div>
</template>
<style>
@media only screen and (max-width: 850px) {
.titles
{
  margin-left: 20px !important;
}
}
.welcome
{
  margin-left: 20px !important;
  margin-right: 0 !important;
}
</style>
<style scoped>
.show {
  display: flex !important;
  justify-content: center;
}
#bars-icon {
  visibility: hidden;
}
#bars-icon:hover {
  cursor: pointer;
}
@media only screen and (max-width: 850px) {
  #bars-icon {
    visibility: visible;
  }
  .nav-items {
    flex-direction: column;
    padding-left: 0 !important;
    background-color: rgba(0, 0, 0, 0.511) !important;
  }
  .nav-item {
    display: none;
  }
  .heading {
    margin-left: 0 !important;
  }
  .button {
    display: none !important;
  }
  .search-icon {
    display: none !important;
  }
}
.search-icon {
  color: white;
  scale: 1.5;
  height: 10px;
}
hr {
  display: block;
  height: 1px;
  border: 0;
  border-top: 1px solid #282828;
  margin: auto;
  padding: 0;
  width: 90%;
}
.navbar-container {
  width: 100%;
  background-color: rgb(0, 0, 0);
}
.nav-items {
  display: flex;
  justify-content: center;
  list-style-type: none;
  text-decoration: none;
}
.nav-item {
  margin: 20px;
  margin-top: 20px;
  text-decoration: none;
}
a {
  text-decoration: none;
  color: rgb(255, 255, 255);
  text-transform: uppercase;
  font-size: 18px;
  /* font-family: 'Montserrat', sans-serif; */
  font: 20px/1.33 Montserrat, Verdana, sans-serif;
  letter-spacing: 1.6px;
}
.nav-item:hover {
  scale: 1.2;
  transition: ease-in-out 200ms;
}
.heading {
  color: white;
  font-family: "Montserrat", sans-serif;
  font-family: "Playfair Display", serif;
  font-size: 44px;
  padding: 5px;
  margin: 0;
  align-items: center;
  width: 170vh;
  margin-left: 170px;
}
.button {
  align-items: right;
  display: flex;
  border-radius: 20px;
  border-width: 0;
  align-items: center;
  text-align: center;
  justify-content: center;
  width: 120px;
  height: 40px;
  background-color: #008573;
  color: white;
  font-weight: 500;
  font-size: 18px;
  transition: 200ms;
}
.button:hover {
  background-color: #0a4f51;
  cursor: pointer;
}
.heading-container {
  display: flex;
  justify-content: center;
  margin-right: 100px;
  margin-left: 100px;
}
.button-container {
  align-self: center;
}
</style>
