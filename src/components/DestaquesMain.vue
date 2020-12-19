<template>
  <div class="destaquesMain">
    <h1>Produtos em Destaque</h1>
    <div class="cards">
      <DestaquesTemplate :gadgets="galaxyFold" id="firstchild"/>
      <DestaquesTemplate :gadgets="galaxyTab" />
      <DestaquesTemplate :gadgets="galaxyNote20"  id="lastchild"/>
    </div>
  </div>
</template>

<script>
import DestaquesTemplate from "../assets/template/DestaquesTemplate";

export default {
  data() {
    return {
      
      galaxyFold: {
        img: "galaxyfold.jpg",
        model: "Galaxy Z Fold2 5G Mystic Black",
        serial: "M-F456FDSD6F7J",
        specs_line_1: "Dobrado, é um celular. Aberto, é um tablet",
        specs_line_2: "Flexível para infinitas possibilidades",
        specs_line_3: "Bateria dupla feita para durar o dia todo",
        price: "R$ 13.999,00",
        portion: "ou 12x de R$ 1.166,58 sem juros",
      },
      galaxyTab: {
        img: "galaxytab.jpg",
        model: "Galaxy Tab S7 LTE Preto",
        serial: "SM-M3H5B67Z1M0",
        specs_line_1: "LCD LTPS de 120 hz",
        specs_line_2: "S Pen com latência ultrabaixa",
        specs_line_3: "Bateria inteligente de 8.000 mha",
        price: "R$ 6.599,00",
        portion: "ou 12x de R$ 549,00 sem juros",
      },
      galaxyNote20: {
        img: "galaxynote.jpg",
        model: "Galaxy Note20 Mystic Bronze 256GB",
        serial: "SM-M3H5B67Z1M0",
        specs_line_1: "Tela infinita",
        specs_line_2: "Compartilhamento de bateria sem fio",
        specs_line_3: "Caneta S Pen",
        price: "R$ 13.999,00",
        portion: "ou 12x de R$ 1.166,58 sem juros",
      },
      
    };
  },

  components: {
    DestaquesTemplate,
  },

};
</script>

<style scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: Arial, Helvetica, sans-serif;
}
.destaquesMain{
  max-width: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
}
h1{
  font-weight: bold;
  text-align: center;
  padding-bottom: 50px;
}
.cards{
  display: flex;
  align-items: center;
  justify-content: center;
}
@media(max-width: 650px){
  .destaquesMain{
    align-items: flex-start;
    justify-content: flex-start;
  }
  .cards{
    max-width: 100%;
    align-items: flex-start;
    justify-content: center;
    overflow: scroll;
  }
  
  #firstchild{
    margin-left: 15px;
  }
  #lastchild{
    margin-right: 15px;
  }
}
</style>