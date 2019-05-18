<template>
  <div id="app">
    <nav class="navbar" role="navigation" aria-label="main navigation">
      <div class="navbar-brand">
        <a class="navbar-item" href="https://bulma.io">
          <img src="https://bulma.io/images/bulma-logo.png" width="112" height="28">
        </a>

        <a
          role="button"
          class="navbar-burger burger"
          aria-label="menu"
          aria-expanded="false"
          data-target="navbarBasicExample"
        >
          <span aria-hidden="true"></span>
          <span aria-hidden="true"></span>
          <span aria-hidden="true"></span>
        </a>
      </div>

      <div id="navbarBasicExample" class="navbar-menu">
        <div class="navbar-start">
          <a class="navbar-item r-item">
            <router-link to="/">Home</router-link>
          </a>

          <a class="navbar-item r-item">
            <router-link to="faq">Features</router-link>
          </a>
          <a class="navbar-item r-item">
            <router-link to="faq">About</router-link>
          </a>
          <a class="navbar-item r-item">
            <router-link to="faq">FAQ</router-link>
          </a>

          <div class="navbar-item has-dropdown is-hoverable">
            <a class="navbar-link">More</a>

            <div class="navbar-dropdown">
              <a class="navbar-item">About</a>
              <a class="navbar-item">Jobs</a>
              <a class="navbar-item">Contact</a>
              <hr class="navbar-divider">
              <a class="navbar-item">Report an issue</a>
            </div>
          </div>
        </div>

        <div class="navbar-end">
          <div class="navbar-item">
            <div class="buttons">
              <a class="button is-primary is-outlined">
                <span class="icon">
                  <i class="fa fa-download"></i>
                </span>
                <strong>Sign up</strong>
              </a>
              <a class="button is-light">Log in</a>
            </div>
          </div>
        </div>
      </div>
    </nav>
    <!-- <div class="nav has-shadow">
      <div class="container">
        <div class="nav-left">
          <a class="nav-item">My Company</a>
        </div>

        <span class="nav-toggle">
          <span></span>
          <span></span>
          <span></span>
        </span>

        <div class="nav-right nav-menu">
          <router-link to="/" class="nav-item r-item">Home</router-link>
          <router-link to="faq" class="nav-item r-item">Features</router-link>
          <router-link to="faq" class="nav-item r-item">About</router-link>
          <router-link to="faq" class="nav-item r-item">FAQ</router-link>

          <div class="nav-item">
            <p class="control">
              <a class="button is-primary is-outlined">
                <span class="icon">
                  <i class="fa fa-download"></i>
                </span>

                <span>JOIN NOW</span>
              </a>
            </p>
          </div>
        </div>
      </div>
    </div>-->
    <router-view>test</router-view>
  </div>
</template>

<script>
export default {
  // eslint-disable-next-line
  name: "App"
};
</script>

<style lang='sass'>
@import '../node_modules/bulma/bulma.sass'
@import 'mq'

.navbar
  background-color: #383838
  a:hover
    color:gray
.nav-left  a
  color: #fff
  font-weight: bold
a.r-item  
  color: #C1C1C1
  padding: 0.5rem 1.75rem
  +mobile
    color:gray
    &:hover
      background-color: #F1F1F1



</style>
