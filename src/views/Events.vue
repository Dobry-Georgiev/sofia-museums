<script>
import Navbar from "@/components/navbar.vue";
import Footer from "@/components/footer.vue";

export default {
  name: "Events",
  components: {
    Navbar,
    Footer,
  },
};
</script>
<template>
  <div class="home">
    <Navbar />
    <section id="home">
      <div class="titles">
        <h1 class="title">Събития</h1>
      </div>
    </section>

    <div class="welcome">
      <h1>Тук можете да намерите информация за предстоящи събития в Софийските музеи</h1>
      <p>Към момента няма активни събития</p>
    </div>

    <Footer />
  </div>
</template>
<style scoped>
#home {
  height: 100vh;
  max-width: 100%;
  background-image: url("../assets/images/theatre2.png");
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
.welcome {
  color: white;
  margin-top: 200px;
  margin-bottom: 200px;
  margin-left: 300px;
  margin-right: 300px;
}
</style>
