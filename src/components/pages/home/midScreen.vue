<template>
  <div class="midScreen">
    <div class="abovewater">
      <Post :floatright="false" class="post" />
      <Post class="post" />
    </div>
    <Waves />
    <div class="underwater">
      <div class="postflex">
        <Post class="post" />
        <Post class="post" />
        <Post class="post" />
        <Post class="post" />
      </div>
    </div>
  </div>
</template>

<script>
import Post from "../../shared/post/Post";
import Waves from "../../shared/waves/Waves";

export default {
  components: {
    Post,
    Waves
  }
};
</script>

<style scoped lang="scss">
@import "../../../scss/colors.scss";

.midScreen {
  background-color: $tertiaryColor;
  box-shadow: 0px -10px 50px 5px;
  text-align: center;
  width: 100%;
}

.underwater {
  background-color: $mainColor;
}

.postFlex2 {
  width: 100%;
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: center;
  align-items: center;
  overflow: visible;
  padding: 2% 0;

  .post {
    margin: 1%;
  }
}
</style>