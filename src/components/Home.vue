<template>
  <div class="home">
    <section class="hero is-medium">
        <div class="hero-body">
          <div class="container">
          <div class="columns">
            <!--<div class="column is-one-fifth"> 
              <img src="../assets/images/imageOfMe.jpeg" id="image" class="is-rounded">
            </div>-->
            <div class="column">
              <h1 class="title has-text-left is-paddingless main-title">
                {{ title }}
              </h1>
            </div>
          </div>
          <div class="column is-two-thids is-paddingless">
            <h2 class="subtitle has-text left">
              {{ subtitle }}
            </h2>
          </div>
        <router-link to="/contact" class="button is-link">
          <span>Contact</span>
        </router-link>
      </div>
      </div>
     </section>

    <section class="section">
      <div class="container">
        <div class="columns is-desktop">
          <div class="column is-1-desktop has-text-centered">
            <span class="icon">
              <i class="fas fa-check-circle"></i>
            </span>
          </div>
          <div class="column is-one-second-desktop">
            <p class="title">
              {{ titlesection }}
            </p>
          </div>
          <div class="column">
            <p class="subtitle">
              {{ subsection }}
            </p>
          </div>
        </div>
      </div>
    </section>

    <section class="section">
      <div class="container">
        <h1 class="title has-text-centered">Skills</h1>
        <h2 class="subtitle has-text-centered">I have worked with various different technologies in my self-driven projects</h2>
        <div class="columns">
          <div class="column is-one-third">
            <div class="card has-shadow">
              <div class="card-content">
                <p class="title has-text-centered">
                  <span class="icon">
                    <i class="fab fa-angular"></i>
                  </span>
                </p>
                <p class="subtitle has-text-centered">
                  Angular5
                </p>
              </div>
            </div>
          </div>
          <div class="column is-one-third">
            <div class="card has-shadow">
              <div class="card-content">
                <p class="title has-text-centered">
                  <span class="icon">
                    <i class="fab fa-vuejs"></i>
                  </span>
                </p>
                <p class="subtitle has-text-centered">
                  Vue.js
                </p>
              </div>
            </div>
          </div>
          <div class="column is-one-third">
            <div class="card has-shadow">
              <div class="card-content">
                <p class="title has-text-centered">
                  <span class="icon">
                    <i class="fab fa-android"></i>
                  </span>
                </p>
                <p class="subtitle has-text-centered">
                  Android app development
                </p>
              </div>
            </div>
          </div>
        </div>
        <div class="columns">
          <div class="column is-one-third">
            <div class="card has-shadow">
              <div class="card-content">
                <p class="title has-text-centered">
                  <span class="icon">
                    <i class="fab fa-html5"></i>
                  </span>
                </p>
                <p class="subtitle has-text-centered">
                  HTML5
                </p>
              </div>
            </div>
          </div>
          <div class="column is-one-third">
            <div class="card has-shadow">
              <div class="card-content">
                <p class="title has-text-centered">
                  <span class="icon">
                    <i class="fab fa-css3-alt"></i>
                  </span>
                </p>
                <p class="subtitle has-text-centered">
                  Css frameworks
                </p>
              </div>
            </div>
          </div>
          <div class="column is-one-third">
            <div class="card has-shadow">
              <div class="card-content">
                <p class="title has-text-centered">
                  <span class="icon">
                    <i class="fab fa-node-js"></i>
                  </span>
                </p>
                <p class="subtitle has-text-centered">
                  Node.js
                </p>
              </div>
            </div>
        </div>
      </div>
     
        <router-link to="/about" class="button is-link is-outlined btn">
          <span>More info</span>
        </router-link>
          
    </div>
    </section>
    <section class="section">
      <div class="container"> 
        <div class="columns">
          <div class="column is-one-third">
           <h1 class="title">Contact</h1>
            <a href="http://gmail.com">
              <span classs="icon">
                <i class="far fa-envelope"></i>
              </span>
            </a>
          </div>
          <div class="column is-two-thirds">
            <h1 class="title">Find me</h1>
            <a href="http://github.com">
              <span class="icon">
                <i class="fab fa-linkedin"></i>
              </span>
            </a>
            <a href="http://linkedin.com">
            <span class="icon">
              <i class="fab fa-github"></i>
            </span>
            </a>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>

export default {
  name: 'home',
  data () {
    return {

      title: 'Passionate software developer at your service',
      subtitle: 'I have a strong backround in web-development especially with frontend tools and technologies. ',
      titlesection: 'My skills include front-end and backend development technologies.',
      subsection: ''
  
    }
    
  },

    methods: {
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="sass" scoped>

@import '../mq.sass'

.hero
  .button
    margin-top: 30px
    background-color: $pri-color
    &:hover
      border: 1px solid $pri-color
      background-color: #fff
      color: $pri-color
      cursor: pointer

.section
  .fa-check-circle
    font-size: 48px
    color: $pri-color
  
.section
  .title
    font-size: 25px
    margin-top: 0px
    

  .btn
    background: $pri-color
    color: #fff
    position: relative
    display: grid
    grid-template-columns: auto auto auto auto

    &:hover
      background: #fff
      color: $pri-color

.is-rounded
    border-radius: 100%
    height: 190px
    width: 190px

.main-title
  margin-top: 70px
</style>
