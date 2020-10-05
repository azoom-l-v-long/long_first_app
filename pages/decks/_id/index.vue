<template>
  <h1>My Decks detail {{ $route.params.id }}</h1>
</template>

<script>
export default {
  validate({ params, query, store }) {
    if (isNaN(params.id)) return false // if the params are valid
    return true // will stop Nuxt.js to render the route and display the error page
  },
}
</script>
