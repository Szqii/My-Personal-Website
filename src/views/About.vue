<template>
  <div class="container-fluid d-flex align-items-center">
    <div class="container-fluid mt-5 ml-0 mr-0 d-flex flex-row justify-content-around">
      
      <div class="desc d-flex flex-column text-center align-items-center">
        <h1 class="mb-5">About me !</h1>
        <p>📸 My name is <span>Sezgi ALTAN.</span></p>
        <p>💪🏼 20 years old.</p>
        <p>📌 Currently living in Antalya due to pandemic.</p>
        <p>
          📚 Second-year student in computer engineering at Pamukkale
          University, Denizli.
        </p>
        <p>
          🎮 Interested in playing online competitive games,taking
          photos,editing Youtube videos,sci-fi movies and TV series.
        </p>
        <p>
          🎯 My biggest aim is being very comprehensive developer but as
          starting, I am trying to learn front-end technologies.
        </p>
        <p>📞 Contact me via social media platforms from icons above.</p>
        <p>
          📨 <a href="mailto: szqii.altn@gmail.com"> szqii.altn@gmail.com</a>
        </p>
        <router-link to="/" tag="button" class="btn mb-3 p-3 ">
          Go to welcome page</router-link
        >
        <router-link to="/projects" tag="button" class="btn p-3 ">
          Check out my simple projects!</router-link
        >
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
* {
  font-weight: 800;
}
a {
  color: #520365;
}
.btn {
  width: 50%;
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
    box-shadow: 600px 0 0 #520365 inset;
  }
}
</style>
