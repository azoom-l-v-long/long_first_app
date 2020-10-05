<template>
  <div id="">
    <h1>Your decks, please enter number of deck to show:</h1>
    <input
      class="form-control"
      type="text"
      v-model="deckId"
      placeholder="Please enter deckId"
    />
    <button class="btn-success" @click="showDeck()">Go to Deck</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      deckId: '1',
    }
  },
  methods: {
    showDeck() {
      // this.$route.push('decks/'+this.deckId)
      this.$router.push(`/decks/${this.deckId}`)
    },
  },
}
</script>
