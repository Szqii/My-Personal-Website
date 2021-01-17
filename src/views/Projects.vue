<template>
  <div class="container-fluid d-flex flex-column align-items-center">
    <h1 class="title mt-5 mb-5 text-center">Here is my some projects !</h1>
    <div class="container-fluid mt-5 row d-flex justify-content-center">
      <div class="grid-item">
        <img src="../assets/todo.png" alt="" />
        <button class="app-links">
          <a href="https://easiest-todo-app.netlify.app/" target="_blank">Try it out!</a>
        </button>
        <button class="app-source">
          <a href="https://github.com/Szqii/Easiest-Todo-App" target="_blank"
            >See source code</a
          >
        </button>
        <p class="p-1">A simple to-do app using local storage.</p>
      </div>
      <div class="grid-item">
        <img src="../assets/vuerld.png" alt="" /><button class="app-links">
          <a href="https://vuerld.netlify.app/" target="_blank">Try it out!</a>
        </button>
        <button class="app-source">
          <a href="https://github.com/Szqii/Vuerld" target="_blank">See source code</a>
        </button>
        <p class="p-1">
          App that is showing informations of all countries in the world.
        </p>
      </div>
      <div class="grid-item">
        <img src="../assets/wwwa.png" alt="" /><button class="app-links">
          <a href="https://wwwa.netlify.app/" target="_blank">Try it out!</a> !</button
        ><button class="app-source">
          <a href="https://github.com/Szqii/Worldwide-Weather-App" target="_blank"
            >See source code</a
          >
        </button>
        <p class="p-1">App that is showing weather in entered city.</p>
      </div>
      <div class="grid-item">
        <img src="../assets/product.png" alt="" /><button class="app-source">
          <a href="https://github.com/Szqii/Product-App" target="_blank">See source code</a>
        </button>
        <p class="p-1">App that provides product operations on the database.</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
img {
  width: 100%;
}
.grid-item {
  position: relative;
  width: 40%;

  margin: 25px;
  box-shadow: 0px 0px 24px 8px rgba($color: #520365, $alpha: 0.4);
  @media (max-width: 1000px) {
    width: 100%;
  }
  button {
    padding: 0.5rem;
    z-index: 1;
    position: absolute;
    bottom: 50px;
    color: rgba($color: #520365, $alpha: 0.8);
    background: #fff;
    border: none;
    border-radius: 10px;
    transition: 0.3s;
    box-shadow: 0 0 24px 8px rgba($color: #520365, $alpha: 0.4);
    &:hover {
      color: #fff;
      transform: scale(1.1);
      background-color: rgba($color: #000, $alpha: 0.5);
    }
    @media (min-width: 350px) and (max-width: 500px) {
      padding: 0.3rem;
    }
    @media (max-width: 350px) {
      padding: 0.1rem;
    }
  }
  .app-links {
    left: 50px;
    @media (max-width: 500px) {
      bottom: 70px;
      left: 5px;
    }
  }
  .app-source {
    right: 50px;
    @media (max-width: 500px) {
      bottom: 70px;
      right: 5px;
    }
  }
}
</style>
