<template>
  <div id="app">
    <nav class="navbar" role="navigation" aria-label="main navigation">
      <div class="navbar-brand">
        <a class="navbar-item" href="#">
          <i class="fas fa-laptop-code is-primary"></i>
          <!-- <i class="fas fa-hippo"></i> -->
        </a>
        <div class="navbar-item">
          <h2>
            <strong>Elaine Lee</strong>
          </h2>&nbsp;
          &nbsp;
          &nbsp;
          <p>Front-End Web Developer</p>
        </div>

        <a
          role="button"
          class="navbar-burger burger"
          aria-label="menu"
          aria-expanded="false"
          data-target="navbarBasicExample"
          v-on:click="toggleNav"
          v-bind:class="{'is-active': isActive}"
        >
          <span aria-hidden="true"></span>
          <span aria-hidden="true"></span>
          <span aria-hidden="true"></span>
        </a>
      </div>

      <div id="navbarBasicExample" class="navbar-menu" v-bind:class="{'is-active': isActive}">
        <div class="navbar-start">
          <a class="navbar-item r-item">
            <router-link to="/">Home</router-link>
          </a>

          <a class="navbar-item r-item">
            <router-link to="faq">Portfolio</router-link>
          </a>
          <a class="navbar-item r-item">
            <router-link to="faq">About</router-link>
          </a>
          <a class="navbar-item r-item">
            <router-link to="faq">Contact</router-link>
          </a>
        </div>

        <div class="navbar-end">
          <div class="navbar-item">
            <div class="buttons">
              <a class="button is-primary is-outlined">
                <span class="icon">
                  <i class="fab fa-github"></i>
                </span>
                <a href="https://github.com/elaineleeworld" target="_blank">
                  <strong>GitHub</strong>
                </a>
              </a>
              <a class="button is-primary is-outlined">
                <span class="icon">
                  <i class="fab fa-codepen"></i>
                </span>
                <a href="https://codepen.io/elaineleeworld/" target="_blank">
                  <strong>CodePen</strong>
                </a>
              </a>
            </div>
          </div>
        </div>
      </div>
    </nav>

    <router-view></router-view>

    <footer class="footer is-primary">
      <div class="container">
        <div class="columns">
          <div class="column">
            <p>
              Crafted with &#10084; in Los Angeles, California &nbsp;
              &nbsp;@All Rights Reserved. &nbsp;
              &nbsp;Powered by Elaine Lee
            </p>
          </div>
        </div>
        <div class="column has-text-center">
          <a class="icon" href="https://www.linkedin.com/in/elaineleeworld/" target="_blank">
            <i class="fab fa-linkedin"></i>
          </a>
          <a class="icon" href="https://github.com/elaineleeworld/" target="_blank">
            <i class="fab fa-github"></i>
          </a>
          <a class="icon" href="https://codepen.io/elaineleeworld/" target="_blank">
            <i class="fab fa-codepen"></i>
          </a>
        </div>
      </div>
    </footer>
  </div>
</template>

<script>
export default {
  // eslint-disable-next-line
  name: "App",
  data: function() {
    return {
      isActive: false
    };
  },
  methods: {
    toggleNav: function() {
      this.isActive = !this.isActive;
    }
  }
};
</script>

<style lang='sass'>
@import '../node_modules/bulma/bulma.sass'
@import 'mq'

.navbar
  a:hover
    color:gray
.nav-left  a
  color: #fff
  font-weight: bold
.navbar-item 
      color: #000
a.r-item  
  color: #C1C1C1
  padding: 0.5rem 1.75rem
  +mobile
    color:gray
    &:hover
      background-color: #F1F1F1
footer
  background-color: $primary !important
  color: #fff
  height: 30px
  text-align: center
  padding: 3rem 1.5rem 8rem !important

  .icon 
    color: #fff
    margin-left: 20px
    font-size: 30px

.fa-hippo, .fa-laptop-code
    background-color: transparent
    color: #00d1b2
    font-size: 30px


</style>
