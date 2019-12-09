<template>
  <div class="topscreen">
    <div id="background" />
    <h1 class="screentitle">Planos</h1>
    <div class="topScreenFlex">
      <PackCard class="cards" />
      <PackCard class="cards" />
      <PackCard class="cards" />
    </div>
  </div>
</template>

<script>
import PackCard from "../../shared/packCard/PackCard";

export default {
  components: {
    PackCard
  }
};
</script>

<style scoped lang="scss">
@import "../../../scss/colors.scss";

.topscreen {
  #background {
    z-index: -1;
    position: fixed;
    background-image: url("../../../assets/ocean.jpg");
    background-attachment: fixed;
    width: 100%;
    height: 100%;
    background-position: center center;
    filter:brightness(0.6);
  }

  height: 100%;
  width: 100%;
  overflow: hidden;
}

.screentitle {
  text-align: center;
  font-size: 7vh;
  text-transform: uppercase;
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen,
    Ubuntu, Cantarell, "Open Sans", "Helvetica Neue", sans-serif;
  font-weight: 300;
  padding-top: 3%;
  padding-bottom: 3%;
  margin-bottom: -5%;
  color: $forthColor;
}

.topScreenFlex {
  height: 100%;
  display: flex;
  justify-content: space-around;
  align-items: center;
  .cards {
    margin-top: -10%;
  }
}

@media only screen and (max-width: 730px) {
  .topScreenFlex{
    flex-direction: column;
    margin-top: 10vh;
    height:80%;
  }
  .screentitle{
    margin-top: 5vh;
    margin-bottom: 15vh;
  }

  .cards{
    margin: 10vh;
  }

  .topscreen{
    height: 200%;
    display:inline-block;
  }

}


</style>