<template>
  <div class="navbarmobile">
      <div class="navbar">
          <ul>
              <span id="close"><input id="closeButton" type="submit" value="X" @click="closebar"></span>
              <li class="option">Telefonia</li>
              <li class="option" >Tablets</li>
              <li class="option" >TV e Áudio </li>
              <li class="option" >Eletrodomésticos </li>
              <li class="option" >Informática </li>
              <br>
              <hr>
              <br>
              <li>Promoções </li>
              <li>Minha Conta </li>
              <br>
              <hr>
          </ul>
      </div>
  </div>
</template>

<script>
export default {
data(){

},
methods:{
    closebar(){
        document.querySelector(".navbarmobile").style.display = "none"
    }
}
}
</script>

<style scoped>
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
.navbarmobile{
    width: 100%;
    height: 100vh;
    position: fixed;
    z-index: 10000;
    top: 0;
    left: 0;
    display: none;
    justify-content: flex-end;
    background: rgba(0,0,0,0.7);
    transition: all .2s linear;
}
.navbar{
    background: #fff;
    width: 360px;
    height: 100%;
    display: flex;
    align-items: flex-start;
}
#close{
    width: 100%;
    display: flex;
    justify-content: flex-end;
    padding-bottom: 10px;
    padding-right: 10px;
    font-size: 25px;
    font-weight: 400;
    color: #000;
}
#closeButton{
    cursor: pointer;
    background: transparent;
    border: none;
    outline: none;
}
.navbar ul{
    list-style: none;
    width: 100%;
}
.navbar ul li{
    padding: 15px 10px;
    font-size: 1.4em;
    letter-spacing: 0.1px;
    cursor: pointer;
}
.option::after{
    content: '>';
    float: right;
    font-weight: 500;
}



</style>