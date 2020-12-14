<template>
  <div class="destaques">
    <div class="cards">
      <div class="card">
        <div class="imagem">
          <img v-bind:src="gadgets.img" alt="gadget" />
        </div>
        <div class="cor">
          <div class="opcao"></div>
          <div class="opcao"></div>
        </div>
        <div class="modelo">
          <h3>
              {{gadgets.model}}
          </h3>
          <p>{{gadgets.serial}}</p>
        </div>
        <div class="descricao">
          <ul>
            <li>{{gadgets.specs_line_1}}</li>
            <li>{{gadgets.specs_line_2}}</li>
            <li>{{gadgets.specs_line_3}}</li>
          </ul>
        </div>
        <div class="valor">
          <p>{{gadgets.price}}</p>
          <p>{{gadgets.portion}}</p>
        </div>
        <div class="button">
          <button>COMPRAR</button>
        </div>
      </div>
    </div>
     
  </div>
 
</template>

<script>
export default {
  props: {
    img: String,
    model: String,
    serial: String,
    specs_line_1: String,
    specs_line_2: String,
    specs_line_3: String,
    price: String,
    gadgets: Object
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
.destaques {
  width: 100%;
  height: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: flex-start;
  margin-bottom: 50px;
}
.destaques h1 {
  margin-top: 10px;
  margin-bottom: 30px;
  text-align: center;
  font-size: 45px;
  font-weight: bold;
}
.cards {
  display: flex;
  align-items: center;
  justify-content: center;
}
.card {
  border: solid 1px transparent;
  width: 400px;
  height: 900px;
  display: flex;
  flex-direction: column;
  align-items: center;
  margin: 20px 25px;
  cursor: pointer;
}
.card:hover {
  border: solid 1px #000;
}
.imagem {
  width: 200px;
  height: 200px;
  margin-top: 100px;
  display: flex;
  align-items: center;
  justify-content: center;
}
.imagem img {
  width: 100%;
  height: 100%;
}
#especial {
  width: 300px;
}
.cor {
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  padding-top: 85px;
  padding-bottom: 30px;
}
.opcao {
  width: 18px;
  height: 18px;
  border: solid 1px gainsboro;
  border-radius: 50px;
  margin: 0 10px;
}
.opcao:nth-child(1) {
  background-color: #000;
}
.opcao:nth-child(2) {
  background-color: rgb(255, 157, 214);
}
.modelo h3 {
  font-size: 22px;
  font-weight: bold;
  text-align: center;
  padding-bottom: 50px;
}
.modelo p {
  text-align: center;
  font-size: 12px;
  color: rgb(0, 0, 0, 0.6);
}
.modelo p::after {
  content: "";
  width: 270px;
  height: 1px;
  display: block;
  background: gainsboro;
  margin: 12px auto;
}
.descricao {
  margin-bottom: 100px;
  width: 70%;
}
.descricao li {
  font-size: 11px;
  color: rgb(0, 0, 0, 0.5);
  padding-bottom: 5px;
  margin-left: 30px;
}
.valor {
  text-align: center;
}
.valor p:nth-child(1) {
  font-size: 25px;
  font-weight: 600;
}
.valor p:nth-child(2) {
  font-size: 15px;
  color: rgb(0, 138, 224);
}
.button {
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  margin-top: 10px;
}
.button button {
  width: 70%;
  height: 50px;
  border-radius: 50px;
  border: none;
  background-color: rgb(0, 0, 165);
  color: #fff;
  font-size: 15px;
  font-weight: 700;
  outline: none;
  cursor: pointer;
}
.button button:hover {
  background-color: rgb(0, 0, 83);
}

/* RESPONSIVE */
@media (max-width: 650px) {
  .destaques h1 {
    font-size: 1.7rem;
  }
  .destaques {
    width: 100%;
  }
  .cards {
    display: flex;
    align-items: center;
    justify-content: flex-start;
    position: relative;
    margin: 0;
    padding: 0;
    overflow: scroll;
    transition: 1s;
  }
  .card {
    padding-left: 40px;
    padding-right: 40px;
    width: 320px;
  }
  .card:nth-child(1) {
    margin: 20px;
  }
}
</style>