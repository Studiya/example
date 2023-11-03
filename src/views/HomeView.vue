<template>
  <!-- <main>
    <TheWelcome />
  </main> -->
  <div>{{ foo }}</div>
</template>

<script>
// import TheWelcome from '../components/TheWelcome.vue'
export default {
  data() {
    return {
      foo: 1,
      qux: 2
    }
  },
  created() {
    this.foo = 3
    console.log(this.foo)
  },
  mounted() {
    this.$el
    this.foo = 2
    console.log(this.foo)
  },
  watch() {},
  computed: {
    bar() {
      return this.foo + this.qux
    }
  }
}
</script>
