<template>
  <div class="categories">
    <div class="line">
      <div class="img">
        <span>Smartphones</span>
        <img src="../assets/images/smartphone.jpg" alt="" />
      </div>
      <div class="img">
        <span>TV e Áudio</span>
        <img src="../assets/images/tv.png" alt="" />
      </div>
    </div>
    <div class="line">
      <div class="img">
        <span>Tablets</span>
        <img src="../assets/images/tablet.jpg" alt="" />
      </div>
      <div class="img">
        <span>Smartwatches</span>
        <img src="../assets/images/relogio.jpg" alt="" />
      </div>
    </div>
    <div class="line">
      <div class="img">
        <span>Geladeiras</span>
        <img src="../assets/images/geladeira.png" alt="" />
      </div>
      <div class="img">
        <span>ArCondicionado</span>
        <img src="../assets/images/arcondicionado.png" alt="" />
      </div>
    </div>
    <div class="line">
      <div class="img">
        <span>Notebooks</span>
        <img src="../assets/images/notebook.jpg" alt="" />
      </div>
      <div class="img">
        <span>Aspiradores</span>
        <img src="../assets/images/aspirador.png" alt="" />
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: Arial, Helvetica, sans-serif;
}
.categories {
  padding: 50px 50px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  width: 100%;
  height: 100%;
}
.line {
  display: flex;
  align-items: center;
  justify-content: center;
  border: none;
  width: 100%;
  margin-bottom: 12px;
  width: 100%;
}
.categories span {
  position: absolute;
  z-index: 1;
  padding: 40px;
  font-size: 2rem;
  font-weight: bold;
  border: none;
}
.img {
  position: relative;
  width: 660px;
  height: 320px;
  margin: 5px 8px;
  cursor: pointer;
  transition: 0.5s;
}
.img img {
  width: 100%;
  height: 100%;
}

/* RESPONSIVE */

@media (max-width: 1080px) {
  .categories {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    width: 100%;
    margin: 20px 0px;
    padding: 0px 30px;
  }
  .line {
    width: 100%;
  }
  .img {
    margin: 0px 5px;
    width: 400px;
    height: 220px;
  }
  .img span {
    font-size: 1.2rem;
    padding: 25px;
  }
}
@media (max-width: 770px) {

  .img {
    margin: 0px 5px;
    width: 400px;
  }
}
@media (max-width: 650px) {
  .line {
    flex-direction: column;
    margin: 0;
  }
  .img {
    width: 100%;
    margin: 10px 0px;
  }
}
</style>