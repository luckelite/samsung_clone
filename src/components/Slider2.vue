<template>
  <div class="slider2">
    <div class="images">
      <img src="../assets/images/watch3.jpg" alt="watch" />
      <img src="../assets/images/budslive.jpg" alt="budslive" />
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
.slider2 {
  display: flex;
  justify-content: center;
  align-items: center;
  max-width: 100%;
  height: 400px;
  margin-top: 50px;
  margin-bottom: 100px;
}
.images {
  position: relative;
  max-width: 100%;
  height: 440px;
  display: flex;
  justify-content: center;
}
.images img {
    padding: 10px;
}

</style>