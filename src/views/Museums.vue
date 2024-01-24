<script>
import Navbar from "@/components/navbar.vue";
import Footer from "@/components/footer.vue";

export default {
  name: "Home",
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
        <h1 class="title">Списък с музеи</h1>
      </div>
    </section>

    <div class="welcome">
      <h1>Добре дошли в София - градът на културата и историята</h1>
      <p>
        Изпъстрен с богато наследство, градът предлага множество музейни
        съкровища, които пригряват посетителите си с удивителни експозиции и
        изключителни истории. Ето петте най-вълнуващи музейни посещения в София:
      </p>
      <br />
      <br />
      <h2>Национален исторически музей</h2>
      <p>
        Заплетен в историята на България, този музей предоставя вълнуващ поглед
        върху етапите от борбата за свобода и разцвета на българската култура.
      </p>
      <br>
      <br>
      <h2>Национален художествен музей:</h2>
      <p>
        Прекрачете портите на този музей и се потопете в света на изкуството,
        представен в шедьоври от български и световни майстори, които разкриват
        вдъхновяваща гама от стилове и периоди.
      </p>
      <br>
      <br>
      <h2>Национален археологически музей:</h2>
      <p>
        Разкрийте тайните на древните цивилизации, докосвайки се до
        археологически находки, които проследяват еволюцията на човечеството в
        българските земи.
      </p>
      <br>
      <br>
      <h2>Музей на социализма:</h2>
      <p>
        Пътувайте във времето и се насладете на уникален поглед върху
        социалистическата епоха в България, разглеждайки предмети и събития,
        които са оставили следи в съзнанието на нацията.
      </p>
      <br>
      <br>
      <h2>Музей на природата и науката:</h2>
      <p>
        Отворете очите си за чудесата на природата и науката в този музей,
        където интерактивни експонати и динамични изложби ще ви накарат да се
        възхищавате на красотата и величието на света около нас.
      </p>
      <br>
      <br>
      <p>
        Заповядайте в София и се потопете в богатата културна сцена на града
        чрез тези невероятни музеи, които ще ви пренесат в историята, изкуството
        и науката.
      </p>
    </div>

    <Footer />
  </div>
</template>
<style scoped>
#home {
  height: 100vh;
  max-width: 100%;
  background-image: url("../assets/images/center.png");
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
  margin-left: 500px;
  margin-right: 600px;
}
</style>
