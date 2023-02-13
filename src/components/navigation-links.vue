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
    <a
      href="https://timesync.novocall.co/mecaca/mecaca-sales-meeting/"
      target="_blank"
      rel="noreferrer noopener"
      class="navigation-links-link"
    >
      {{ text1 }}
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
    text1: {
      type: String,
      default: 'Schedule a demo',
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
.navigation-links-link {
  margin-left: var(--dl-space-space-twounits);
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
  .navigation-links-link {
    margin-left: 0;
    margin-bottom: var(--dl-space-space-unit);
  }
}
@media(max-width: 479px) {
  .navigation-links-root-class-name10 {
    display: flex;
  }
}
</style>
