<template>
  <div id="main">
    <Header />
    <div id="pseudoHeader" />
    <TopScreen id="top"/>
    <MidScreen id="mid"/>
    <Footer/>
  </div>
</template>

<script>
import Header from "../../shared/header/Header";
import TopScreen from "../../pages/home/topScreen";
import MidScreen from "../../pages/home/midScreen";
import Footer from "../../shared/footer/Footer"

export default {
  components: {
    Header,
    TopScreen,
    MidScreen,
    Footer
  }
};
</script>

<style lang="scss">
@import "../../../scss/colors.scss";

html,
body {
  height: 100%;
  width: 100%;
  box-sizing: border-box;
}


#main {
  height: 90%;
}

#pseudoHeader {
  height: 15%;
}

#midScreen {
  height: 100%;
}
</style>