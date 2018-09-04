<template>
  <div id="app">
    <h1>Scoreboard</h1>
    <section class="scoreboard">
    <section class="team-1">
      <TeamName />
    </section>
    <section class="team-2">
      <TeamName />
    </section>
  </section>
  </div>
</template>

<script>

import TeamName from './components/TeamName.vue'
export default {
  name: 'app',
  components: {
    TeamName,

  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.scoreboard {
  display: flex;
  justify-content: space-around;
}

.team-1 {
  height: 20em;
  width: 33%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}


.team-2 {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
</style>
