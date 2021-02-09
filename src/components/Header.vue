<template>
  <div class="header">
    <NavBarMobile />
    <div class="components-header">
      <div class="logo">
        <p>SAMSUNG</p>
      </div>
      <div class="nav">
        <ul>
          <li>Telefonia</li>
          <li>Tablets</li>
          <li>TV e Áudio</li>
          <li>Eletrodomésticos</li>
          <li>Informática</li>
        </ul>
      </div>
      <div class="users">
        <ul>
          <li>Promoções</li>
          <li><img src="../assets/images/user.png" alt="user" /></li>
          <li><img src="../assets/images/market.png" alt="market" /></li>
          <li><img src="../assets/images/search.png" alt="search" /></li>
          <li><img id="iconMenu" src="../assets/images/menu.png" alt="" @click="openbar"/></li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
import NavBarMobile from './NavBarMobile'
export default {
  components: {
    NavBarMobile
  },
  methods: { 
    openbar(){
        document.querySelector(".navbarmobile").style.display = "flex"
    }
  }
}
</script>

<style scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: Arial, Helvetica, sans-serif;
}
.header {
  width: 100%;
  height: 80px;
  display: flex;
  align-items: center;
  justify-content: center;
}
.components-header{
  width: 100%;
  height: 100%;
  display: flex;
  align-items: center;
  padding: 0 20px;
}
.logo {
  width: 300px;
  height: 100%;
  display: flex;
  align-items: center;
}
.logo > img {
  display: none;
}
.logo p {
  font-weight: bold;
  font-size: 20px;
  height: 100%;
  width: 100%;
  display: flex;
  align-content: center;
  align-items: center;
}
.nav {
  display: flex;
  width: 100%;
  height: 100%;
  align-items: center;
}
.nav ul {
  display: flex;
  align-items: center;
}
.nav ul li {
  font-size: 13px;
  font-weight: bold;
  display: flex;
  align-items: center;
  border-radius: 30px;
  padding: 7px 10px;
}
.nav ul li:hover {
  background-color: black;
  color: white;
  cursor: pointer;
}
.users {
  width: 500px;
  height: 100%;
  display: flex;
}
.users ul {
  width: 100%;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: flex-end;
}
.users ul li {
  list-style: none;
  cursor: pointer;
}

.users ul li:nth-child(1),
.users ul li:nth-child(2),
.users ul li:nth-child(3){
  margin: 20px;
}
.users ul li:nth-child(4){
  margin-left: 20px;
}

.users ul li:nth-child(1) {
  border-radius: 30px;
  padding: 7px 10px;
  font-weight: bold;
  font-size: 13px;
  margin-left: 0;
}
.users ul li:nth-child(1):hover {
  background-color: #000;
  color: #fff;
  cursor: pointer;
  border-radius: 50px;
}
#iconMenu {
  display: none;
}

/* RESPONSIVE */

@media(max-width: 650px){
  .header {
    width: 100%;
    height: 50px;
  }
  .logo {
    width: 100%;
    height: 100%;
  }
  .logo p {
    font-size: 1.2rem;
    font-weight: 800;
    padding: 5px;
  }
  .nav {
    display: none;
  }
  .users ul{
    width: 100%;
  }
  .users ul li:nth-child(1),
  .users ul li:nth-child(2) {
    display: none;
  }
 .users ul li:nth-child(3),
 .users ul li:nth-child(4){
   margin-left: 5px;
 }
 .users ul li img:nth-child(3),
 .users ul li img:nth-child(4){
   width: 25px;
   height: 25px;
 }
  #iconMenu {
    display: initial;
    cursor: pointer;
    width: 25px;
    height: 25px;
    margin-left: 20px;
  }
}
@media(max-width: 1080px){
  .header {
    width: 100%;
    height: 50px;
  }
  .logo {
    width: 100%;
    height: 100%;
  }
  .logo p {
    font-size: 1.2rem;
    font-weight: 800;
    padding: 5px;
  }
  .nav {
    display: none;
  }
  .users ul{
    width: 100%;
  }
  .users ul li:nth-child(1),
  .users ul li:nth-child(2) {
    display: none;
  }
 .users ul li:nth-child(3),
 .users ul li:nth-child(4){
   margin-left: 5px;
 }
 .users ul li img:nth-child(3),
 .users ul li img:nth-child(4){
   width: 25px;
   height: 25px;
 }
  #iconMenu {
    display: initial;
    cursor: pointer;
    width: 25px;
    height: 25px;
    margin-left: 20px;
  }
}
</style>