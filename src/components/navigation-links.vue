<template>
  <nav class="navigation-links-nav" v-bind:class="rootClassName">
    <a
      href="https://reviews.mecaca.my/#/"
      target="_blank"
      rel="noreferrer noopener"
      class="navigation-links-text"
    >
      {{ text }}
    </a>
  </nav>
</template>

<script>
export default {
  name: 'NavigationLinks',
  props: {
    rootClassName: String,
    text: {
      type: String,
      default: 'Login',
    },
  },
}
</script>

<style scoped>
.navigation-links-nav {
  flex: 0 0 auto;
  display: flex;
  align-items: center;
  flex-direction: row;
}
.navigation-links-text {
  text-decoration: none;
}








.navigation-links-root-class-name10 {
  display: none;
}
@media(max-width: 767px) {
  .navigation-links-nav {
    align-items: flex-start;
    flex-direction: column;
  }
  .navigation-links-text {
    margin-bottom: var(--dl-space-space-unit);
  }
}
@media(max-width: 479px) {
  .navigation-links-text {
    font-size: 18px;
    font-style: normal;
    font-weight: 700;
    margin-right: var(--dl-space-space-unit);
    margin-bottom: 0px;
  }
  .navigation-links-root-class-name10 {
    display: flex;
  }
}
</style>
