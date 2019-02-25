<template>
  <div class="counter">
    <h1>{{ msg }} - ({{ num }} * {{ multiply }}) = {{ total }}</h1>
    <div>
      <button v-on:click="clickCounter">{{ btnText }}</button>
      <button v-on:click="calculate">calculate</button>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'Counter',
    props: {
      msg: String,
      multiply: String
    },
    data: function() {
      return {
        num: 0,
        total: 0,
        btnText: 'Click Counter',
      }
    },
    methods: {
      clickCounter: function() {
        alert(`Clicked ${this.num} times`)
      },
      calculate: function() {
        this.num++;
        this.total = this.num * this.multiply;
      },
    },
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
button {
  border: solid .1rem #41B883;
  border-radius: .1rem;
  color: #41B883;
  background-color: #ffffff;
  margin: .3rem;
  padding: .3rem;
}

.counter {
  color: #41B883;
}
</style>
