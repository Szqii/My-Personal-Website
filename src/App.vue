<template>
  <div class="container-fluid p-0 ">
    <Header></Header>
          <transition name="fade" mode="out-in">
      <router-view></router-view>
    </transition>
  </div>
</template>

<script>
import Header from "./components/Header";
export default {
  components: {
    Header,
  },
};
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Yusei+Magic&display=swap");
* {
  font-family: "Yusei Magic", sans-serif;
}
body {
  padding: 0;
  margin: 0;
  box-sizing: border-box;

  background-image: radial-gradient(
    circle 993px at 0.5% 50.5%,
    rgba(137, 171, 245, 0.37) 0%,
    rgba(245, 247, 252, 1) 100.2%
  );

  &::-webkit-scrollbar-track {
    border-radius: 10px;
    background-color: #f5f7fc;
  }

  &::-webkit-scrollbar {
    width: 14px;
    background-color: #f5f7fc;
  }

  &::-webkit-scrollbar-thumb {
    border-radius: 10px;

    background-color: #2f2f2f;
  }
}
.fade-enter{
  opacity: 0;
}
.fade-enter-active{
  transition: opacity .5s ease-out;
}
.fade-leave{
  opacity: 1;
}
.fade-leave-active{
  opacity: 0;
  transition: opacity .5s ease-out;
}
</style>
