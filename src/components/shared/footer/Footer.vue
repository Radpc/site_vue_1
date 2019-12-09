<template>
  <div class="footer">
    <ul>
      <h1>Redes</h1>
      <li>Facebook</li>
      <li>Twitter</li>
      <li>Instagram</li>
    </ul>
    <ul>
      <h1>Redes</h1>
      <li>Facebook</li>
      <li>Twitter</li>
      <li>Instagram</li>
    </ul>

    <div class="rights">
      <p>© Copyright Matheus M. </p>
      <p>Private and fair use</p>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped lang="scss" >
@import "../../../scss/colors.scss";

.footer {
  width: 100%;
  display: flex;
  justify-content: space-around;
  align-content: center;
  align-items: center;
  background-color: $darkContrast;
  box-sizing: border-box;

  ul {
    padding: 2vw;
    flex-grow:0.2;
    h1 {
      font-size: 2vw;
      font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen,
        Ubuntu, Cantarell, "Open Sans", "Helvetica Neue", sans-serif;
      margin-bottom: 1vw;
      padding-bottom: 0.3vw;
      border-bottom: 3px solid $forthColor;
      color: $highlight;
    }
    li {
      font-size: 1.2vw;
      margin: 0.2vw 0;
      color: $mainColor;
      font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen,
        Ubuntu, Cantarell, "Open Sans", "Helvetica Neue", sans-serif;
    }
    li:before {
      content: "- ";
    }
  }


  .rights{
    color:$forthColor;
    flex-shrink: 5;

    text-align: center;
  
    p{
      margin:0.4vw 0;
    }
  
  }
}
</style>>
