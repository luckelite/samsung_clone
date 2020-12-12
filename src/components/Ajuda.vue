<template>
  <div class="ajuda">
    <h1>Precisa de ajuda?</h1>

    <div class="cards">
      <div class="card">
        <div class="imagem">
          <img src="../assets/images/call.png" alt="" />
        </div>
        <div class="titulo">
          <p>Atendimento Loja Online</p>
        </div>
        <div class="texto">
          <p>
            Para informações referentes à sua compra, nosso atendimento está
            disponível de segunda a sexta, exceto feriados nacionais das 08h às
            20h.
          </p>
        </div>
        <div class="vermais">
          <p>0800 007 2611</p>
        </div>
      </div>

      <div class="card">
        <div class="imagem">
          <img src="../assets/images/email.png" alt="" />
        </div>
        <div class="titulo">
          <p>Suporte por Chat ou E-mail</p>
        </div>
        <div class="texto">
          <p>
            Envie suas dúvidas por e-mail ou entre em contato conosco por chat,
            nossos especialistas técnicos estão disponíveis para solucionar tudo
            sobre seu produto.
          </p>
        </div>
        <div class="vermais">
          <p>VEJA MAIS</p>
        </div>
      </div>

      <div class="card">
        <div class="imagem">
          <img src="../assets/images/libras.png" alt="" />
        </div>
        <div class="titulo">
          <p>Atendimento em Libras</p>
        </div>
        <div class="texto">
          <p>
            Conecte-se com um atendente fluente em LIBRAS e receba assistência
            técnica do seu produto Samsung via videoconferência.
          </p>
        </div>
        <div class="vermais">
          <p>VEJA MAIS</p>
        </div>
      </div>

      <div class="card">
        <div class="imagem">
          <img src="../assets/images/remoto.png" alt="" />
        </div>
        <div class="titulo">
          <p>Suporte instalação Remota</p>
        </div>
        <div class="texto">
          <p>
            Tudo o que precisa para começar a desfrutar de seu novo Samsung.
            Confira os tutoriais para os seus primeiros passos ou entre em
            contato com nosso suporte. Verifique produtos elegíveis.
          </p>
        </div>
        <div class="vermais">
          <p>VEJA MAIS</p>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: Arial, Helvetica, sans-serif;
}
.ajuda{
    width: 100%;
    height: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: flex-start;
    margin-bottom: 50px;
}
.ajuda h1{
    margin-bottom: 50px;
    font-weight: bold;
}
.cards{
    display: flex;
    align-items: center;
    justify-content: center;
}
.card{
    background-color: rgb(248,248,248) ;
    height: 550px;
    width: 300px;
    text-align: center;
    padding: 30px;
    margin: 10px;
    border: none;
    border-radius: 0;
}
.imagem{
    padding: 30px;
    margin-bottom: 20px;
}
.titulo{
    font-weight: bold;
    font-size: 1rem;
    margin-bottom: 30px;
}
.texto{
    font-weight: 200;
    height: 200px;
    color: rgb(82, 82, 82);
}
.vermais{
    font-size: 14px;
    font-weight: 600;
    color: rgb(82, 82, 82);
    cursor: pointer;
}


</style>