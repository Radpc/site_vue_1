<template>
  <div>
    <div class="packcard">
      <img
        class="packimage"
        src="https://icon-library.net/images/boat-icon-png/boat-icon-png-10.jpg"
        alt
      />
      <p class="packname">{{ packname }}</p>
      <p class="packdesc">{{ packdesc}}</p>
      <p class="packprice">{{ packprice }}</p>
    </div>
  </div>
</template>

<script>
export default {
  data: function() {
    return {
      packname: "Plano marítitmo",
      packdesc: "Um plano para voce viajar bem pelos mares de manaus!",
      packprice: "300"
    };
  }
};
</script>

<style scoped lang="scss" >
@import "../../../scss/colors.scss";

.packcard {
  display: flex;
  flex-direction: column;
  align-content: center;
  border-radius: 10%;
  background-color: rgba(10, 10, 10, 0.5);
  border: 3px solid $forthColor;
  height: 15em;
  width: 15em;
  padding: 5% 1%;
  justify-content: space-around;
  transition:opacity 0.2s ease;

  .packimage {
    width: 60%;
    height: 60%;
    align-self: center;
    filter: invert(80%) sepia(14%) saturate(4059%) hue-rotate(352deg) brightness(98%) contrast(81%);    
  }

  .packname {
    text-align: center;
    font-size: 2em;
    text-transform: capitalize;
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen,
      Ubuntu, Cantarell, "Open Sans", "Helvetica Neue", sans-serif;
    font-weight: 400;
    color: $tertiaryColor;
  }

  .packdesc {
    padding-bottom: 1em;
    padding-top: 0.2em;
    text-align: center;
    font-size: 1vw;
    color: $tertiaryColor;
  }
  .packprice {
    text-align: center;
    font-size: 1.5em;
    font-weight: 500;
    color: $tertiaryColor;
  }

  .packprice::before {
    content: "R$ ";
  }
}

.packcard:not(:hover){
  opacity:0.8;
}

</style>>
