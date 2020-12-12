<template>
  <div class="app">
    <Header />
    <Carousel />
    <FreteGratis />
    <Categories />
    <Destaques />
    <Ajuda />
    <ProdEServ />
    <Footer />

  </div>
</template>

<script>
import Header from "./components/Header";
//import Slider from "./components/Slider";
import Carousel from './components/Carousel'
import FreteGratis from "./components/FreteGratis";
import Categories from "./components/Categories";
import Destaques from "./components/Destaques";
import Ajuda from './components/Ajuda'
import ProdEServ from './components/ProdEServ'
import Footer from './components/Footer'
//import Slider2 from './components/Slider2'


export default {
  name: "app",
  components: {
    Header,
    Carousel,
    FreteGratis,
    Categories,
    Destaques,
    Ajuda,
    ProdEServ,
    Footer,
  },
};
</script>

<style>
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
.app {
  background-color: #fff;
  display: flex;
  flex-direction: column;
  justify-content: center;
  max-width: 100%;
  overflow: hidden;
}
</style>