<template>
  <div class="hello" style="text-align: center">
    <h1>Hello Sapadi</h1>
    <p>Latihan 1</p>
    <input type="text" placeholder="input your name ..." v-model="namamu" />
    <p>{{ namamu }}</p>
    <button @click="greet(namamu)">Say Hi</button>
    <button @click="pass(namamu)">Send to Manajemen</button>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  data() {
    return {
      namamu: 'Sapadi'
    };
  },
  props: {
    msg: String
  },
  methods: {
    greet(namamu) {
      alert("Hello! "+ namamu);
    },
    pass(namamu) {
      this.$emit("fromChild", namamu)
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
