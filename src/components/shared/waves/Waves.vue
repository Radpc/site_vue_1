<template>
  <section class="waves">
    <div class="wave wave1" alt></div>
    <div class="wave wave2" alt />
    <div class="wave wave3" alt />
  </section>
</template>

<script>
export default {};
</script>

<style scoped lang="scss" >
@import "../../../scss/colors.scss";
.waves {
  padding-top: 1em;
  position: relative;
  overflow: hidden;
  width: 100%;
  height: 5em;
  background-color:$tertiaryColor;
}

.wave {
  position: absolute;
  width: 100%;
  height: 100%;
  filter: invert(100%) invert(18%) sepia(26%) saturate(3377%) hue-rotate(167deg) brightness(96%) contrast(76%);
  animation: animate 50s linear infinite;
  background-image: url(../../../assets/wave.png);
  background-size: 100% 100%;
}

.wave1{
  opacity:1;
  animation-delay: -2s;
  animation: animate 60s linear infinite;
}

.wave2{
  opacity:0.6;
  animation-delay: -3s;
  animation: animate 30s linear infinite;
}

.wave3{
  opacity:0.5;
  animation-delay: -5s;
  animation: animate 50s linear infinite;
}



@keyframes animate {
  0% {
    background-position-x: 0;
  }

  100% {
    background-position-x: 10000px;
  }
}
</style>