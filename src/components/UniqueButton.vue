<template>

<button @click="doesNothing">Reverse M, T, H, A, W, V, U, O, I, and X too because i'm dope </button>
</template>

<script>
export default {
  name: 'UniqueButton',
  methods: {
      doesNothing: function() {
          console.log("Ziz does nothing!")
      }
  }
}
</script>


