<template>
<div class="container">
  <hr/>
 <div class="footer">
  <div class="pages-container">
    <h3 style="margin-bottom: 0;">Полезни връзки</h3>
    <div style="display: flex;">
    <ul class="pages">
      <li>
        <router-link to="/">
      Начало
    </router-link>
      </li>
      <li>
        <router-link to="/музеи">
      Музеи
    </router-link>
      </li>
      <li>
        <router-link to="/събития">
      Събития
    </router-link>
      </li>
    </ul>
    <ul class="pages2">
      <li>
        <router-link to="/галерия">
      Галерия
    </router-link>
      </li>
      <li>
        <router-link to="/контакти">
      Контакти
    </router-link>
      </li>
    </ul>
  </div>
</div>

  <div class="contacts-container">
      <ul class="contacts">
      <li class="mini-header">Свържете се с нас</li>
        <li>
          <a href="tel:+359 28 88 888 888">Телефон: +359 28 88 888 888</a></li>
        <li>Имейл: sofia_museums@domain.com</li>
      </ul>
  </div>
 </div>
</div>
  </template>
  
  <script>
  export default {
    name: 'Footer',
    mounted() {
      
    }
  }
  </script>
  
  <style scoped>
  .container
  {
    margin-left: 200px;
    margin-right: 200px;
  }
  li
  {
    margin-top: 20px;
    text-align: left;
    margin-left: 30px;
    margin-right: 20px;
  }
  .footer
  {
    margin-top: 70px;
    margin-bottom: 70px;
  }
  a
  {
    color: white;
    text-decoration: none;
  }
  .footer
  {
    color: white;
    display: flex;
    justify-content: center;
  }
  .pages-container
  {
    display: flex;
    flex-direction: column;
    margin-right: 100px;
    margin-left: 100px;
  }
  .pages2
  {
    list-style-type: none;
    text-decoration: none;
    padding-left: 0;
  }
  .pages
  {
    list-style-type: none;
    text-decoration: none;
    justify-content: left;
    display: flex;
    flex-flow: wrap;
    flex-direction: column;
  }
  .contacts-container
  {
    list-style-type: none;
    text-decoration: none;
    margin-right: 200px;
    margin-left: 200px;
  }
  .mini-header
  {
    font-size: 1.2rem;
  }
  .contacts
  {
    list-style-type: none;
    text-decoration: none;
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
  </style>