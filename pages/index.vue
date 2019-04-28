<template>
  <section class="hero is-fullheight">
    <div class="hero-body">
      <div class="container">
        <div class="columns">
          <div class="column is-three-fifths">
            <svg class="icon-bug"><use xlink:href="#icon-bug"></use></svg>
            <h1 class="title is-1 has-text-white is-family-secondary">
              EL BUG FARM
            </h1>
            <h4 class="subtitle is-4 has-text-light">
              We are a multicultural and multidisciplinary web design &amp;
              development firm that specializes in providing solutions to
              organizations of different scales through interactivity, media,
              visual communication, art, and identity.
            </h4>
            <h5 class="subtitle is-5 has-text-danger">New site coming soon!</h5>
            <a
              class="button is-link is-inverted is-outlined"
              href="mailto:info@elbugfarm.com"
            >
              Contact Us
            </a>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import anime from 'animejs'
export default {
  mounted() {
    anime({
      targets: '.icon-bug',
      scale: 1.1,
      rotate: '1turn',
      loop: true,
      direction: 'alternate',
      easing: 'spring(1, 80, 10, 0)'
    })
  }
}
</script>

<style lang="scss" scoped>
.icon-bug {
  height: 100px;
  width: 100px;
  display: inline-block;
  fill: #ff3860;
  margin-bottom: 15px;
}
</style>
