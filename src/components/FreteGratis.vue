<template>
  <div class="freteGratis">
    <div class="components-freteGratis">
      <ul>
        <li><img src="../assets/images/12semjuros.jpg" alt="" /></li>
        <li><img src="../assets/images/fretegratis.jpg" alt="" /></li>
        <li><img src="../assets/images/promotoronline.jpg" alt="" /></li>
        <li><img src="../assets/images/instalacaoremota.jpg" alt="" /></li>
      </ul>
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
.freteGratis {
  width: 100%;
  height: 145px;
  display: flex;
  align-items: center;
  justify-content: center;
  overflow: hidden;
}
.components-freteGratis ul{
  width: 100%;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  list-style: none;
}
.components-freteGratis img:nth-child(1),
.components-freteGratis img:nth-child(2),
.components-freteGratis img:nth-child(3) {
  border-right: solid 2px lightgray;
}
.components-freteGratis img:nth-child(1),
.components-freteGratis img:nth-child(2),
.components-freteGratis img:nth-child(3),
.components-freteGratis img:nth-child(4){
  overflow: hidden;
}

/* RESPONSIVE */

@media(max-width: 650px){
   .freteGratis {
    width: 100%;
    height: 200px;
    display: flex;
    align-items: center;
    justify-content: center;
  }
  .components-freteGratis{
    width: 100%;
    position: relative;
    display: flex;
    align-items: center;
    overflow: hidden;
  }
  .components-freteGratis ul{
    display: flex;
    align-items: center;
    justify-content: flex-start;
    overflow: scroll
  }
  .components-freteGratis img:nth-child(1){
    padding-left: 50px;
  }

  .components-freteGratis img:nth-child(1),
  .components-freteGratis img:nth-child(2),
  .components-freteGratis img:nth-child(3),
  .components-freteGratis img:nth-child(4){
    border: none;
    overflow: hidden;
  }
}
</style>