<template>
  <div class="ajuda">
    <h1>Precisa de ajuda?</h1>
    <div class="cards">
      <AjudaTemplate :helper="atendimento" id="firstchild"/>
      <AjudaTemplate :helper="suporte"  />
      <AjudaTemplate :helper="libras" />
      <AjudaTemplate :helper="remoto" id="lastchild"/>
    </div>
  </div>
</template>

<script>
import AjudaTemplate from "../assets/template/AjudaTemplate";

export default {
  data() {
    return {

      atendimento: {
        image: "call.png",
        title: "Atendimento Loja Online",
        text:
          "Para informações referentes à sua compra, nosso atendimento está disponível de segunda a sexta, exceto feriados nacionais das 08h às 20h.",
        more: "0800 007 2611",
      },
      suporte: {
        image: "email.png",
        title: "Suporte por Chat ou E-mail",
        text:
          " Envie suas dúvidas por e-mail ou entre em contato conosco por chat, nossos especialistas técnicos estão disponíveis para solucionar tudo sobre seu produto.",
        more: "VEJA MAIS",
      },
      libras: {
        image: "libras.png",
        title: "Atendimento em Libras",
        text:
          "Conecte-se com um atendente fluente em LIBRAS e receba assistência técnica do seu produto Samsung via videoconferência.",
        more: "VER MAIS",
      },
      remoto: {
        image: "remoto.png",
        title: "Suporte instalação Remota",
        text:
          "Tudo o que precisa para começar a desfrutar de seu novo Samsung. Confira os tutoriais para os seus primeiros passos ou entre em contato com nosso suporte. Verifique produtos elegíveis.",
        more: "VER MAIS",
      },
    };
  },
  components: {
    AjudaTemplate,
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
.ajuda{
  display: flex;
  flex-direction: column;
  align-items: center;
  max-width: 100%;
}
h1{
  font-weight: bold;
  padding-bottom: 50px;
}
.cards{
  display: flex;
  align-items: center;
}

@media(max-width: 1180px){
  
}
@media(max-width: 770px){
  .ajuda{
    margin-bottom: 0;
  }
  .cards{
    display: flex;
    flex-direction: column;
    width: 100%;
    padding: 10px;
    
  }
  h1{
  font-weight: bold;
  font-size: 1.5em;
}
}

</style>