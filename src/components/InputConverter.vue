<template>
<br>
<h2>Your sucky text:</h2>
<textarea v-model="message" placeholder="add multiple lines" rows="4" cols="50"></textarea>
<br>
<h2>Your new, better text:</h2>
{{messageConverted}}

</template>

<script>
export default {
  name: 'InputConverter',
  data() {
      return {
        message: 'Rad! I am a string'
      }
  },
  computed: {
      messageConverted() {
        const betterUppercaseR = 'Я';
        const betterLowercaseR = 'я';

        const newString = this.message.replace('r', betterLowercaseR).replace('R', betterUppercaseR)

        return newString;
      }
  },
  methods: {
  }
}
</script>


