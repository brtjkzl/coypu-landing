<template>
  <header>
    <github-corner></github-corner>
    <h2>{{ title }}</h2>
    <router-link to="/" class="text-lead link-muted">
      Back to the homepage
    </router-link>
  </header>
</template>

<script>
import GitHubCorner from './GitHubCorner'

export default {
  name: 'navbar',
  components: {
    'github-corner': GitHubCorner
  },
  props: {
    title: {
      required: true
    }
  }
}
</script>

<style scoped>
@import '../variables.css';

header {
  margin-bottom: var(--spacing-unit);
}

h2 {
  margin-top: 0;
  margin-bottom: calc(var(--spacing-unit) / 2);
}
</style>
