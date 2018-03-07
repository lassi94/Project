<template>
  <div id="app">
    <nav class="navbar has-shadow" role="navigation">
      <div class="container">
        <div class="navbar-brand">
          <router-link to="/" class="navbar-item">Company</router-link>

        <div class="navbar-burger" v-on:click="toggleNav" v-bind:class="{ 'is-active':isActive }">
          <span></span>
          <span></span>
          <span></span>
        </div>
        </div>

        <div class="navbar-menu" v-bind:class="{ 'is-active':isActive }">
          <div class="navbar-start">
            <router-link to="/" class="navbar-item">Home</router-link>
            <router-link to="/about" class="navbar-item">About</router-link>
          </div>
          <div class="navbar-end">
            <a class="navbar-item">
              <span class="icon" id="icon-git">
                <i class="fab fa-github"></i>
              </span>
            </a>
            <a class="navbar-item">
              <span class="icon" id="icon-linked">
                <i class="fab fa-linkedin"></i>
              </span>
            </a>
            <a class="navbar-item">
              <router-link to="/contact" class="button is-outlined">
                <span id="contact">Contact me</span>
              </router-link>
            </a>
          </div>
        </div>
      </div>
    </nav>

    <transition name="router-anim">
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
  name: 'App',
  data(){
    return{
      isActive:false

      }
    },
       methods: {
      toggleNav: function(){
        this.isActive = !this.isActive;
    }
  }
}
</script>

<style lang="sass">

@import '../node_modules/bulma/bulma.sass'
@import 'mq.sass'
@import url('https://fonts.googleapis.com/css?family=Montserrat:400,700')

body
  font-family: Montserrat

.navbar a
  color: $pri-color
  &:hover
    background-color: #FFFFFF
    color: #000000

.footer
  background-color: $pri-color

.fa-github
  font-size: 30px

.fa-linkedin
  font-size: 30px

.navbar-end
  .button
    color: $pri-color
    border: 1px solid 
    &:hover
      background-color: $pri-color
      color: #fff
      cursor: pointer

.navbar
  .navbar-burger
    color: $pri-color

    &:hover
     background-color: #fff

.app 
  position: fixed
  width: inherit

.router-anim-enter-active
  animation: coming 1s
  animation-delay: .5s
  opacity: 0

.router-anim-leave-active
  animation: going 1s

@keyframes going
  from
    transform: translateX(0)

  to
    transform: translateX(-50px)
    opacity: 0

@keyframes coming
  from
    transform: translateX(-50px)
    opacity: 0

  to
    transform: translateX(0)
    opacity: 1

</style>
