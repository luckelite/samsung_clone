<template>
  <div class="prodEServ">
      <div class="items">
        <div class="item">
          <div class="title">
            <h1>PRODUTOS E SERVIÇOS</h1>
          </div>
          <div class="left">
            <a href="#">Smartphones</a>
            <a href="#">Tablet</a>
            <a href="#">Watches</a>
            <a href="#">Áudio</a>
            <a href="#">Acessórios</a>
          </div>
          <div class="right">
            <a href="#">Informática</a>
            <a href="#">TV e Áudio</a>
            <a href="#">Geladeira</a>
            <a href="#">Lavadoras e Secadoras</a>
            <a href="#">Ar condicionado</a>
          </div>
        </div>

        <div class="item">
          <h1>LOJA ONLINE</h1>
          <a href="#">Promoções</a>
          <a href="#">FAQ Loja Online</a>
        </div>

        <div class="item">
          <h1>SUPORTE</h1>
          <a href="#">Fale Conosco</a>
          <a href="#">Chat Online</a>
          <a href="#">Email</a>
          <a href="#">Centro de Serviços</a>
          <a href="#">Comunidade</a>
        </div>

        <div class="item">
          <h1>COMPANHIA</h1>
          <a href="#">Lojas Samsung</a>
          <a href="#">Promoção</a>
          <a href="#">Quem Somos</a>
          <a href="#">Notícias</a>
          <a href="#">Corporate</a>
          <a href="#">Corporate Citizenship</a>
          <a href="#">Investidores</a>
          <a href="#">Celular Legal</a>
        </div>
      </div>
  </div>
</template>

<style scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
.prodEServ {
  display: flex;
  align-items: center;
  justify-content: center;
  max-width: 100%;
  height: 100%;
  margin-top: 50px;
}
.items {
  position: relative;
  display: flex;
  width: 100%;
  height: 100%;
}
.item {
  height: 320px;
  width: 100%;
  border: 1px solid rgb(217,217,217);
  border-right: none;
}
.item:nth-child(1) {
  display: grid;
  grid-template-columns: 300px 300px;
  grid-template-rows: 50px auto;
  grid-template-areas:
    "title title"
    "left right";
    border-left: none;
}
.title {
  grid-area: title;
  display: flex;
  align-items: center;
}
.left {
  grid-area: left;
  padding-right: 20px;
}
.right {
  grid-area: right;
}
.item h1 {
  font-size: 1rem;
  padding-left: 20px;
}
.item:nth-child(2) h1, .item:nth-child(3) h1, .item:nth-child(4) h1 {
  padding: 15px 20px;
}
.item:nth-child(4){
  border-right: none;
}
.item a {
  display: flex;
  padding: 6px;
  padding-left: 20px;
  text-decoration: none;
  color: rgb(75, 75, 75);
  font-size: 0.8rem;
}
.item a:hover{
  color: #000;
}

</style>