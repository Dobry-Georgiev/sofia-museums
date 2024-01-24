<script>
import Navbar from "@/components/navbar.vue";
import Footer from "@/components/footer.vue";

export default {
  name: "Home",
  components: {
    Navbar,
    Footer,
  },
  methods: 
  {
    buyTickets: function ()
    {
      alert('The website is under development. Please try again once it is officially published')
    }
  }
};
</script>
<template>
  <div class="home">
    <Navbar />
    <section id="home">
      <div class="titles">
        <h1 class="title">София</h1>
        <h5 class="title">Музеи и култура</h5>
        <button v-on:click="buyTickets()" class="tickets">Билети</button>
      </div>
    </section>
    
    <Footer />
  </div>
</template>
<style scoped>
#home {
  height: 100vh;
  max-width: 100%;
  background-image: url("../assets/images/sofia-1.png");
  background-size: cover;
  background-position: center;
}
.titles {
  display: flex;
  justify-content: left;
  margin-left: 260px;
  padding-top: 250px;
  color: white;
  font-size: 3rem;
  flex-direction: column;
  text-align: left;
  font-family: "Montserrat", sans-serif;
  font-family: "Playfair Display", serif;
}
.title {
  margin: 10px;
}
.tickets
{
  align-items: right;
  display: flex;
  border-radius: 20px;border-width: 0;
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
  margin-left: 5px;
  margin-top: 25px;
}
.tickets:hover
{
  background-color: #0a4f51;
  cursor: pointer;
}
</style>
