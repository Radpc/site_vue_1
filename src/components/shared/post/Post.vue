<template>
  <div class="post">
    <h1>{{ title }}</h1>
    <img v-bind:class="{floatRight : floatright}" :src="image" alt="A cat" />
    <p>{{ desc }}</p>
    <button>{{ buttonDesc }}</button>
  </div>
</template>

<script>
import Cat from "../../../assets/cat.png";

export default {
  props: {
    floatright: Boolean
  },

  data() {
    return {
      title: "Easy to use",
      image: Cat,
      buttonDesc: "Buy",
      desc:
        "Lorem ipsum dolor sit amet consectetur adipisicing elit. Nisi, cupiditate nulla fugit libero earum eligendi veniam a expedita ratione at asperiores voluptatum optio consequatur. Enim aperiam unde voluptatem veniam sint."
    };
  }
};
</script>

<style scoped lang="scss" >
@import "../../../scss/colors.scss";

.post {
  display: inline-block;
  width: 40vw;
  height: 20vw;
  padding: 1%;
  text-align: center;

  h1 {
    margin-top: 3%;
    font-size: 3vw;
    text-align: left;
    color: $forthColor;
  }
  img {
    margin-top: 5%;
    margin-right: 5%;
    border-radius: 50%;
    height: 10vw;
    width: 10vw;
    object-fit: cover;
    transition: border-radius 0.3s ease, transform 0.2s ease;
    float: left;
  }

  .floatRight {
    float: right;
  }

  img:hover {
    border-radius: 25%;
    transform: scale(1.2);
  }

  p {
    margin-top: 5%;
    display: block;
    text-align: center;
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen,
      Ubuntu, Cantarell, "Open Sans", "Helvetica Neue", sans-serif;
  }
  button {
    border: 0;
    font-size: 2vw;
    margin-top: 1vw;
    padding: 0.1vw 2vw;
    background-color: $forthColor;
    color: $mainColor;
    border-radius: 1em;
  }
}
</style>>
