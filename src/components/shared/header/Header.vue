<template>
  <div class="header">

    <div id="pseudoHeader" />
    <div class="logoDiv">
      <img id="imglogo" src="../../../assets/logo.png" />
      <h1 id="title">BoatSym</h1>
      <span id="subtitle">Sailing through the seas</span>
    </div>
    <div class="buttonsDiv">
      <button class="headerButton">
        <a href="#">Home</a>
      </button>
      <button class="headerButton">
        <a href="#">Products</a>
      </button>
      <button class="headerButton">
        <a href="#">About</a>
      </button>
      <button class="headerButton">
        <a href="#">Contact</a>
      </button>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped lang="scss" >
@import "../../../scss/colors.scss";

.header {
  z-index: 100;
  box-sizing: border-box;
  background-color: $tertiaryColor;
  display: flex;
  justify-content: space-around;
  padding: 1.5em;
  flex: 5;
  box-shadow: 0px -20px 40px 30px black;
  position: fixed;
  width: 100%;
  height: 15vh;
  border-bottom-left-radius: 0.3em;
  border-bottom-right-radius: 0.3em;
}

.logoDiv {
  #imglogo {
    height: 100%;
    width: 100%;
    width: auto;
    float: left;
    margin-right: 1vw;
  }

  #title {
    font-size: 5vh;
    vertical-align: middle;
    text-transform: capitalize;
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen,
      Ubuntu, Cantarell, "Open Sans", "Helvetica Neue", sans-serif;
    font-weight: 300;
    letter-spacing: 2px;
    color: $mainColor;
  }

  #subtitle {
    font-size: 1em;
    text-align: center;
    color: $secondaryColor;
  }
  height: 100%;
  flex-grow: 1;
}

.buttonsDiv {
  padding: auto;
  display: flex;
}

.headerButton {
  a {
    text-decoration: inherit;
    color: inherit;
  }
  background-color: #ffffff00;
  //border: 0.07em solid $mainColor;
  border: 0;
  font-size: 1.5em;
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen,
    Ubuntu, Cantarell, "Open Sans", "Helvetica Neue", sans-serif;
  text-transform: uppercase;
  margin: 0 0.3em;
  padding: 0 10px;
  text-transform: capitalize;
  font-weight: 280;
}

.headerButton:hover {
  a {
    color: $highlight;
  }
  background-color: $mainColor;
}

@media only screen and (max-width: 930px) {
  .buttonsDiv {
    display: block;
  }
  .header {
    flex-direction: column;
    justify-content: center;
    font-size:2vw;
  }

  .logoDiv {
    img {
      display: none;
    }
    text-align: center;
    display: inline-block;

    display: inline-block;
  }

  .buttonsDiv {
    margin-top: 1em;
    text-align: center;
  }
}
</style>>
