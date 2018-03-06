<template>
  <div id="app">
    <nav class="navbar has-shadow" role="navigation">
      <div class="container">
        <div class="navbar-brand">
          <router-link to="/" class="navbar-item">Company</router-link>
        </div>

        <div class="navbar-burger">
          <span></span>
          <span></span>
          <span></span>
        </div>

        <div class="navbar-menu">
          <div class="navbar-start">
            <router-link to="/" class="navbar-item">Home</router-link>
            <router-link to="/About" class="navbar-item">About</router-link>
          </div>
          <div class="navbar-end">
            <a class="navbar-item">
              <span class="icon">
                <i class="fab fa-github"></i>
              </span>
            </a>
            <a class="navbar-item">
              <span class="icon">
                <i class="fab fa-linkedin"></i>
              </span>
            </a>
            <a class="navbar-item">
              <a class="button is-outlined is-link">
                <span id="contact">Contact me</span>
              </a>
            </a>
          </div>
        </div>
      </div>
    </nav>

    <transition name="router-animations">
      <router-view/>
    </transition>

    <footer class="footer">
      <div class="container">
        <div class="columns">
          <div class="column">

          </div>
          <div class="column">

          </div>
        </div>
      </div>
    </footer>

  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style lang="sass">

@import '../node_modules/bulma/bulma.sass'
@import 'mq.sass'
@import url('https://fonts.googleapis.com/css?family=Montserrat:400,700');


body
  font-family: Montserrat

.navbar-item
  color: #0052CC

  &:hover
    background: #fff

.footer
  background-color: #0052CC


</style>
