<template>
  <!-- <template :key="key"> -->
  <div class="container-fluid">
    <div class="container d-flex flex-column  align-items-center">
      <div>
        <h1 class="text-center mb-5 hello">
          <span class="wave">👋🏼</span> Hello there
        </h1>
        <h1 class="text-center mb-4 name">
          I'm <span class="my-name">Sezgi ALTAN</span>
        </h1>

        <h1 class="text-center mb-4 typer-js">
          <vue-typer
            :text="text"
            type-delay="100"
            erase-style="backspace"
            caret-animation="blink"
            pre-erase-delay="750"
            erase-delay="70"
          />
        </h1>
      </div>
      <router-link to="/about" tag="button" class="btn mb-3 p-3 ">
        Click here to learn more about me!</router-link
      >
      <router-link to="/projects" tag="button" class="btn p-3 ">
        Check out my simple projects!</router-link
      >
    </div>
  </div>
</template>

<script>
import { VueTyper } from "vue-typer";
export default {
  components: {
    VueTyper,
  },
  data() {
    return {
      text: [
        "📚 CE. Student",
        "📸 Amateur Photographer",
        "💻 Front-end fancier",
        "💚 VueJS Lover",
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
.container {
  margin-top: 100px;
  .my-name {
    color: #520365;
  }
  .typer-js {
    font-size: 36px;
    @media (min-width: 415px) and (max-width: 525px) {
      font-size: 28px;
    }
    @media (min-width: 365px) and (max-width: 415px) {
      font-size: 24px;
    }
    @media (max-width: 365px) {
      font-size: 20px;
    }
  }
  .hello {
    @media (max-width: 350px) {
      font-size: 34px;
    }
  }
  .name {
    @media (max-width: 350px) {
      font-size: 32px;
    }
  }
  .btn {
    width: 30%;
    background: rgba($color: #520365, $alpha: 0.5);
    margin: 20px;
    float: left;
    border: 0px;
    color: #fff;
    box-shadow: 0 0 1px #ccc;
    transition-duration: 0.4s;
    transition-timing-function: linear;
    box-shadow: 0px 0 0 #520365 inset;
    &:hover {
      box-shadow: 400px 0 0 #520365 inset;
    }
    @media (max-width: 1000px) {
      width: 100%;
    }
  }
}
.wave {
  cursor: pointer;
  &:hover {
    animation-name: wave-animation; /* Refers to the name of your @keyframes element below */
    animation-duration: 2s; /* Change to speed up or slow down */
    animation-iteration-count: infinite; /* Never stop waving */
    transform-origin: 90% 90%; /* Pivot around the bottom-left palm */
    display: inline-block;
  }
}

@keyframes wave-animation {
  0% {
    transform: rotate(0deg);
  }
  10% {
    transform: rotate(14deg);
  } /* The following five values can be played with to make the waving more or less extreme */
  20% {
    transform: rotate(-14deg);
  }
  30% {
    transform: rotate(24deg);
  }
  40% {
    transform: rotate(-4deg);
  }
  50% {
    transform: rotate(10deg);
  }
  60% {
    transform: rotate(0deg);
  } /* Reset for the last half to pause */
  100% {
    transform: rotate(0deg);
  }
}
</style>
