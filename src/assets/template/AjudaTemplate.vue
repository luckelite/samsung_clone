<template>
  <div class="ajuda">
    <div class="cards">
      <div class="card">
        <div class="imagem">
          <img :src="require('@/assets/images/' + helper.image )" alt="img" />
        </div>
        <div class="titulo">
          <p>{{ helper.title }}</p>
        </div>
        <div class="texto">
          <p>
            {{ helper.text }}
          </p>
        </div>
        <div class="vermais">
          <p>{{ helper.more }}</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
      image: String,
      title: String,
      text: String,
      more: String,
      helper: Object,
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
.ajuda {
  width: 100%;
  height: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: flex-start;
  margin-bottom: 50px;
}
.ajuda h1 {
  margin-bottom: 50px;
  font-weight: bold;
}
.cards {
  display: flex;
  align-items: center;
  justify-content: center;
}
.card {
  background-color: rgb(248, 248, 248);
  height: 550px;
  width: 300px;
  text-align: center;
  padding: 30px;
  margin: 10px;
  border: none;
  border-radius: 0;
}
.imagem {
  padding: 30px;
  margin-bottom: 20px;
}
.titulo {
  font-weight: bold;
  font-size: 1rem;
  margin-bottom: 30px;
}
.texto {
  font-weight: 200;
  height: 200px;
  color: rgb(82, 82, 82);
}
.vermais {
  font-size: 14px;
  font-weight: 600;
  color: rgb(82, 82, 82);
  cursor: pointer;
}

/* Responsive */
@media(max-width: 1180px){

.card{
  height: 400px;
}
.imagem {
  padding: 10px;
  margin-bottom: 20px;
}
.titulo {
  margin-bottom: 15px;
}
.texto {
  height: 230px;
  color: rgb(82, 82, 82);
}

}
</style>