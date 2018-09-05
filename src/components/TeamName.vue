<template>
  <section class="team">
    <h3>{{ team1name }}</h3>
    <h1>{{ score }}</h1>
    <section class="update-name">
      <p>Update Team 1 Name</p>
      <input type='text' v-model='teamNameInput'>
      <button v-on:click='updateName'>Update</button>
    </section>
    <section class="update-score">
      <p>Update Team 1 Score</p>
      <button v-on:click='addOneToScore'>Add 1</button>
      <button v-on:click='subtractOnefromScore'>Subtract 1</button>
    </section>
  </section>
</template>

<script>
export default {
  name: 'TeamName',
  data: function() {
    return{
      team1name: 'Update your Team Names',
      teamNameInput: '',
      score:0
    }
  },
  methods:{
    updateName:function() {
      this.team1name = this.teamNameInput
    },
    addOneToScore:function() {

      this.score++
    },
    subtractOnefromScore:function() {

      this.score--
    }
  }
}
</script>

<style scoped>
.team {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.update-name {
  display: flex;
}

.update-name p {
  padding: 1em;
}
.update-score {
  display: flex;
}

.update-score p {
  padding: 1em;
}


</style>
