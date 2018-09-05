<template lang="html">
  <section class="update-score">
    <p>Update Team 1 Score</p>
    <button v-on:click='addOneToScore'>Add 1</button>
    <button v-on:click='subtractOnefromScore'>Subtract 1</button>
  </section>

</template>

<script>
export default {
  name: 'TeamScore',
  methods:{
  addOneToScore:function() {
    console.log('plus boom')
  },
  subtractOnefromScore:function() {
    console.log('minus boom')
  }
 }
}
</script>

<style scoped lang="css">
.update-score {
  display: flex;
}

.update-score p {
  padding: 1em;
}
</style>
