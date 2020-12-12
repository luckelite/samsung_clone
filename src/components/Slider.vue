<template>
  <div class="slider">
      <img src="../assets/images/anuncio.png" alt="bf">
      <img src="../assets/images/slider-mobile.jpeg" alt="mobile">
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: Arial, Helvetica, sans-serif;
}
.slider{
    width: 100%;
    height: 430px;
    display: flex;
    align-items: center;
    justify-content: center;
}
.slider img{
    max-width: 100%;
    height: 100%;
}
.slider img:nth-child(2){
    display: none;
}

/* RESPONSIVE */

@media(max-width: 650px){
    .slider {
    width: 100%;
    height: 420px;
    display: flex;
    align-items: center;
    justify-content: center;
    overflow: hidden;
  }
  .slider img:nth-child(1){
    display: none;
  }
  .slider img:nth-child(2){
    display: initial;
  }
  .slider img {
    width: 100%;
    height: 100%;
  }
}
</style>