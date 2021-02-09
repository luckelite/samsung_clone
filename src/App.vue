<template>
  <div id="app">
    <Header />
    <Carousel />
    <CarrouselMobile />
    <FreteGratis />
    <Categories />
    <DestaquesMain />
    <AjudaMain />
    <ProdEServ />
    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header";
//import Slider from "./components/Slider";
import Carousel from "./components/Carousel";
import CarrouselMobile from "./components/CarrouselMobile";
import FreteGratis from "./components/FreteGratis";
import Categories from "./components/Categories";
import DestaquesMain from "./components/DestaquesMain";
import AjudaMain from "./components/AjudaMain";
import ProdEServ from "./components/ProdEServ";
import Footer from "./components/Footer";
//import Slider2 from './components/Slider2'

export default {
  el: "app",
  components: {
    Header,
    Carousel,
    CarrouselMobile,
    FreteGratis,
    Categories,
    DestaquesMain,
    AjudaMain,
    ProdEServ,
    Footer,
  },
};
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
#app {
  background-color: #fff;
  display: flex;
  flex-direction: column;
  justify-content: center;
  max-width: 100%;
  overflow: hidden;
}
@media (max-width: 650px) {
  .slides-mobile {
    /* Componente Carrousel */
    display: initial;
  }
  .slides {
    /* Componente Carrousel-mobile */
    display: none;
  }
}
@media (min-width: 655px) {
  .slides-mobile {
    /* Componente Carrousel */
    display: none;
  }
  .slides {
    /* Componente Carrousel */
    display: initial;
  }
}
</style>