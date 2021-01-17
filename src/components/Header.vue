<template>
  <nav class="navbar sticky-top navbar-expand-lg navbar-light transparent">
    <div class="container" id="navbarNavAltMarkup">
      <div class="navbar-nav d-flex flex-row justify-content-between w-100">
        <div class="empty"></div>
        <div class="contact">
          <a href="https://twitter.com/Szq_ii" target="_blank"
            ><i class="fab fa-twitter fa-2x p-2" />
          </a>
          <a href="https://www.instagram.com/szq_ii" target="_blank"
            ><i class="fab fa-instagram fa-2x p-2" />
          </a>
          <a href="https://www.linkedin.com/in/sezgi-altan/" target="_blank"
            ><i class="fab fa-linkedin-in fa-2x p-2" />
          </a>
          <a href="https://github.com/Szqii" target="_blank"
            ><i class="fab fa-github fa-2x p-2" />
          </a>
          <a
            href="https://discordapp.com/users/284727475047628810/ "
            target="_blank"
            ><i class="fab fa-discord fa-2x p-2" />
          </a>
        </div>
        <div class="home">
          <router-link tag="a" to="/"
            ><i class="fas fa-home fa-2x p-2"></i
          ></router-link>
        </div>
      </div>
    </div>
  </nav>
</template>

<script></script>

<style lang="scss" scoped>
nav {
  border-bottom: 1px solid #232122;
  padding: 1rem;

  .container {
    padding: 0;
  }
  .navbar-nav {
    align-items: center;
    a {
      text-decoration: none;
      color: #232122;
      i {
        transition: 0.2s;
        &:hover {
          transform: scale(1.4);
          color: #520365;
        }
      }
    }
  }
}

.transparent {
  backdrop-filter: blur(5px);
  // border-bottom: 2px solid #121212;
}
</style>
