<template>
  <div class="container">
    <div class="contact-form">
      <h2 id="title" style="color: white">Изпратете запитване</h2>
      <form action="#" method="post">
        <div class="form-group">
          <label for="name">Име</label>
          <input type="text" id="name" name="name" required />
        </div>

        <div class="form-group">
          <label for="email">Е-мейл</label>
          <input type="email" id="email" name="email" required />
        </div>

        <div class="form-group">
          <label for="subject">Запитване</label>
          <textarea id="subject" name="subject" rows="4" required></textarea>
        </div>

        <button v-on:click="sendButton()" type="submit" class="submit-btn">Изпрати</button>
      </form>
    </div>
  </div>
</template>

<script>
export default {
  name: "ContactsForm",
  methods: {
    sendButton: function () {
      alert(
        "Please come back once the website is officially published"
      );
    }
  }
};
</script>

<style scoped>
#title
{
  font-family: "Montserrat", sans-serif;
  font-family: "Playfair Display", serif;
  margin-bottom: 50px;
}
label {
  color: white;
  font-family: "Montserrat", sans-serif;
  font-family: "Playfair Display", serif;;
}
input {
  background-color: rgba(255, 255, 255, 0);
  border-bottom: #f4f4f4;
  color: white !important;
}
.container {
  display: flex;
  justify-content: center;
}
body {
  background-color: #f4f4f4;
  margin: 0;
  display: flex;
  align-items: center;
  justify-content: center;
  height: 100vh;
}

.contact-form {
  /* background-color: #fff; */
  padding: 20px;
  border-radius: 8px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  width: 400px;
  max-width: 100%;
}

.form-group {
  margin-bottom: 20px;
}

label {
  display: block;
  font-size: 1.2rem;
  margin-bottom: 8px;
}

input,
textarea {
  width: 100%;
  padding: 10px;
  border: 1px solid #ddd;
  border-radius: 4px;
  font-size: 14px;
  margin-bottom: 10px;
  box-sizing: border-box;
}

input:focus,
textarea:focus {
  outline: none;
  border-color: #3498db;
}

.submit-btn {
  background-color: #008573;
  color: #fff;
  padding: 10px 15px;
  border: none;
  border-radius: 4px;
  font-size: 16px;
  cursor: pointer;
  transition: background-color 0.3s ease;
}

.submit-btn:hover {
  background-color: #00433a;
}
#subject {
  background-color: rgba(255, 255, 255, 0);
}
textarea
{
  color: white !important;
}
</style>
