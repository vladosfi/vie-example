<template>
  <p>Home !!!!!!!!</p>
  <Button></Button>
</template>
<script>
//import ElButton from '@/components/HelloWorld.vue'
import Button from '@/components/Button.vue'

/* eslint-disable */
export default {
  name: "Home",
  components: {
    Button
  },
  mounted() {
    this.$axios.get('users')
      .then(x => console.log(x.data))
  }
};
</script>

<style></style>
