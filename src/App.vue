<script setup>
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <div>
    <a href="https://vitejs.dev" target="_blank">
      <img src="/vite.svg" class="logo" alt="Vite logo" />
    </a>
    <a href="https://vuejs.org/" target="_blank">
      <img src="./assets/vue.svg" class="logo vue" alt="Vue logo" />
    </a>
  </div>
  <HelloWorld msg="Vite + Vue" />
</template>

<style scoped>
.wrapper {
  width: 400px;
  border: 2px solid black;
  display: inline-flex;
}

.image {
  width: 400px;
}

.header {
  text-align: center;
  font-weight: bold;
  font-size: 2rem;
}

.header h3:hover {
  font-style: italic;
  font-size: 1.1em;
}

.header h3,
.header h4 {
  transition: .3s ease-in-out all;
  margin: 16px;
  font-style: normal;
}

.buttons button:focus,
.buttons button:hover {
  background-color: rgba(200,0,50,.5);
}

.buttons button:active {
  background-color: rgba(50,0,200,.5);
}

.buttons {
  display: block;
}

button {
  padding: 12px;
  font-size: 32px;
}

details {
  margin-left: 24px;
  padding: 10px;
}
.details summary {
  font-size: 20px;
  font-weight: bold;
}


@media only screen and (max-width: 1200px){
  .wrapper {
    background-color: pink;
  }
}
@media only screen and (max-width: 600px){
  .wrapper {
    background-color: purple;
  }
}
@media only screen and (max-width: 425px){
  .wrapper {
    font-weight: normal;
  }
  .wrapper .header h3 {
    font-size: 12px;
  }
  .wrapper .header h4 {
    font-size: 10px !important;
  }
  details {
    display: none;
  }
}
</style>
