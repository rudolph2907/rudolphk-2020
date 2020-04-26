<template>
  <div class="card">
    <div class="card-content" style="padding: 0">
      <img src="~/assets/img/profile-pic.jpg" />
      <ul class="menu">
        <li><nuxt-link to="/">About Me</nuxt-link></li>
        <li><nuxt-link to="/my-work">My Work</nuxt-link></li>
        <li>
          <a href="https://blog.rudolphk.co.za" target="_blank" rel="noreferrer"
            >Blog</a
          >
        </li>
        <li><nuxt-link to="/contact">Contact</nuxt-link></li>
      </ul>
      <div class="social has-text-centered">
        <a
          href="https://twitter.com/rudolphk2907"
          target="_blank"
          class="icon is-large"
        >
          <i class="mdi mdi-twitter mdi-36px"></i>
        </a>
        <a
          href="https://www.linkedin.com/in/rudolphkoegelenberg/"
          target="_blank"
          class="icon is-large"
        >
          <i class="mdi mdi-linkedin mdi-36px"></i>
        </a>
        <a
          href="https://github.com/rudolph2907"
          target="_blank"
          class="icon is-large"
        >
          <i class="mdi mdi-github mdi-36px"></i>
        </a>
      </div>
    </div>
  </div>
</template>

<style>
.menu {
  margin-top: -7px;
}

.menu li a {
  display: block;
  background: #222;
  color: #fff;
  text-transform: uppercase;
  padding: 10px;
  border-bottom: 1px solid #333;
  border-left: 1px solid #222;
  transition: border-width 0.3s ease-in-out;
}
.menu li:last-child a {
  border-bottom: none;
}

.menu li a:hover,
.nuxt-link-exact-active {
  background: #ccc !important;
  border-bottom: 1px solid #ccc;
  border-left: 5px solid #ff0000 !important;
}
</style>
