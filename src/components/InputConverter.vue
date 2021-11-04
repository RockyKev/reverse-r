<template>
<br>
<h2>Your sucky text:</h2>
<textarea v-model="message" placeholder="add multiple lines" rows="4" cols="50"></textarea>
<br>
  <UniqueButton />
<br>
<h2>Your new, better text:</h2>
{{messageConverted}}

</template>

<script>
import UniqueButton from './UniqueButton.vue'

export default {
  name: 'InputConverter',
  components: {
    UniqueButton
  },
  data() {
      return {
        message: 'Life’s but a walking shadow, a poor player, that struts and frets his hour upon the stage, and then is heard no more; it is a tale told by an idiot, full of sound and fury, signifying nothing.'
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


