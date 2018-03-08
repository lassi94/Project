<template>
  <div class="home">
    <section class="hero is-medium">
        <div class="hero-body">
          <div class="container">
          <h1 class="title has-text-left is-paddingless">
            {{ title }}
          </h1>
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
                    <i class="fab fa-angular"></i>
                  </span>
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
              </div>
            </div>
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

      title: 'Ambitious software developer at your service',
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

</style>
