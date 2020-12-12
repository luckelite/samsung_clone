<template>
  <div class="footer">
    <div class="copyright">
      <p>Copyright© 1995-2020 SAMSUNG. Todos os direitos reservados.</p>
      <p>
        SAMSUNG ELETRÔNICA DA AMAZÔNIA LTDA., com sede em Av. dos Oitis, nº
        1.460, Distrito Industrial, Manaus/AM, 69.007-002, inscrita no CNPJ/MF
        sob o nº. 00.280.273/0001-37.
      </p>
      <p>
        LOJA ONLINE SAMSUNG, operada pela SYNAPCOM COMERCIO ELETRÔNICO LTDA, com
        endereço na Avenida Antônio Cândido Machado, 3100, BOX 86 - Cajamar -
        SP, CEP: 07776-550, inscrita no
      </p>
      <p>CNPJ sob o nº. 27.932.734/0002-46 e IE 241.130.824.114.</p>
      <p>Contato Eletrônico para compras na Loja Online.</p>
      <p>
        Esse website é melhor visualizado nas versões Microsoft Internet
        Explorer 11 ou superior e/ou nas últimas versões dos navegadores Google
        Chrome e Mozilla Firefox.
      </p>
    </div>
    <div class="finnaly">
      <ul id="left">
        <li><b>BRASIL/PORTUGUÊS</b></li>
        <li>|</li>
        <li>ACESSIBILIDADE</li>
        <li>TERMOS & CONDIÇÕES LOJA ONLINE</li>
        <li>PRIVACIDADE</li>
        <li>LEGAL</li>
        <li>MAPA DO SITE</li>
      </ul>
      <ul id="right">
        <li>SIGA-NOS</li>
        <li><img src="../assets/images/facebook.png" alt="" /></li>
        <li><img src="../assets/images/twitter.png" alt="" /></li>
        <li><img src="../assets/images/instagram.png" alt="" /></li>
        <li><img src="../assets/images/youtube.png" alt="" /></li>
      </ul>
    </div>
  </div>
</template>

<style scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  color: rgb(97, 97, 97);
}
.footer {
  width: 100%;
  height: 100%;
  display: flex;
  flex-direction: column;
}
.copyright {
  padding-top: 20px;
  padding-left: 20px;
  padding-bottom: 10px;
}
.copyright p {
  font-size: 0.7rem;
}
.finnaly {
  display: flex;
  align-items: center;
  height: 100%;
  border: solid 1px rgb(217, 217, 217);
  border-right: none;
  border-left: none;
}
.finnaly ul {
  display: flex;
  height: 100%;
}
.finnaly ul li {
  list-style: none;
  font-size: 0.7rem;
  cursor: pointer;
}
#left {
  width: 100%;
}
#left li {
  padding: 20px 15px;
}
#right {
  width: 400px;
  align-items: center;
  justify-content: flex-end;
  padding-right: 20px;
}
#right li {
  padding: 20px 10px;
}
</style>