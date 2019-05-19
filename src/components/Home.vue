<template>
  <div class="home">
    <section class="hero">
      <div class="hero-body">
        <div class="container">
          <h1 class="title">{{ heading }}</h1>
          <div class="is-two-thirds column is-paddingless">
            <h2 class="subtitle is-4">{{ subheading }}</h2>
          </div>
          <a class="button is-large is-primary" id="learn">Contact Me</a>
        </div>
      </div>
    </section>

    <section class="section">
      <div class="container">
        <div class="columns pd is-desktop">
          <div class="column is-1 has-text-centered">
            <i class="far fa-lightbulb fa-6x is-primary"></i>
          </div>
          <div class="column is-one-third-desktop has-text-centered">
            <p class="title">
              <strong>I provide superior web development for you so that you can focus on other tasks and your business can succeed.</strong>
            </p>
          </div>
          <div class="column">
            <p>I can create innovative and exciting webpages so that your customers enjoy coming to your site and increase repeat business. From e-commerce to databases and mobile, tablet and desktop friendly designs, your website will be top-notch and user-friendly.</p>
          </div>
        </div>
      </div>

      <div class="columns pd">
        <div class="column">
          <div class="card">
            <div class="card-content">
              <p
                class="title"
              >FullStack Developer creating landing pages, e-commerce CMS, database management, devOps, agile workflow</p>
              <p class="subtitle">Beachbody LLC</p>
            </div>
          </div>
        </div>

        <div class="column">
          <div class="card">
            <div class="card-content">
              <p
                class="title"
              >Front-End Developer creating HTML Banner Ads, custom ReactJS websites, Email Templates, Mobile friendly pages</p>
              <p class="subtitle">Red Interactive Agency</p>
            </div>
          </div>
        </div>

        <div class="column">
          <div class="card">
            <div class="card-content">
              <p
                class="title"
              >Teaching Assistant for Programming course. ReactJS, Javascript, CSS, HTML fundamentals, servers, databases</p>
              <p class="subtitle">UCLA Extension</p>
            </div>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  // eslint-disable-next-line
  name: "Home",
  data() {
    return {
      heading: "Soar to new heights",
      subheading:
        "Have a website that your customers enjoy visiting again and again. Contact me today to see what I can for your website."
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang='sass' scoped>
@import '../mq'

.hero 
  background: url('../assets/clouds.jpg')
  background-size: cover
  
  .title 
    +mobile
      font-weight: bold
    +tablet
      font-size: 2.5rem
    +desktop
      font-size: 4rem
      margin-top: 2.5rem
h2 
  margin: 1.5rem 0 2rem 0 !important

#learn
  +desktop  
    margin-bottom: 2rem
.pd
  +tablet
  padding: 2em 0
</style>
