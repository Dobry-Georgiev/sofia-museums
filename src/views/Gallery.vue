<script>
import Navbar from "@/components/navbar.vue";
import Footer from "@/components/footer.vue";

export default {
  name: "Gallery",
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
        <h1 class="title">Галерия</h1>
        <p>Потопи се в дълбочините на изкуството и илюзиите</p>
      </div>
    </section>

    <div class="gallery">
      <div class="image">
        <img src="@/assets/images/gallery1.jpg" alt="">
      </div>

      <div class="image">
        <img src="@/assets/images/gallery2.jpg" alt="">
      </div>

      <div class="image">
        <img src="@/assets/images/gallery3.webp" alt="">
      </div>

      <div class="image">
        <img src="@/assets/images/gallery4.jpg" alt="">
      </div>

    </div>
    

    <Footer />
  </div>
</template>
<style scoped>
.gallery
{
    margin-top: 200px;
    justify-content: center;
    display: flex;
    margin-left: 200px;
    margin-right: 200px;
    flex-wrap: wrap;
    align-items: center;
}
img
{
    border-radius: 30px;
    max-width: 600px;
    margin-top: 50px;
    margin-bottom: 50px;
    margin-left: 30px;
    margin-right: 30px;
}
#home {
  height: 100vh;
  max-width: 100%;
  background-image: url("../assets/images/gallery.png");
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
