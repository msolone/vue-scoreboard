<template>
  <section>
  <h1>Hello, {{ user }} </h1>
</section>
</template>

<script>
export default {
  name: 'Greetings',
  props: {
    user: String
  }
}
</script>

<style scoped>
h1 {
  color: red;
}

</style>
