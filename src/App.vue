<script setup>
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <header>
<div class="buttons">
  <button class="duplicate">Duplicate last card</button>
  <button class="modifytitle">Change Name</button>
  <button id="deletelastcard">Delete</button>
<div class="btn-wrapper">
  <button href="https://gopsusports.com/sports/football/roster/nicholas--singleton/14065">Nicholas Singleton</button>
</div>
<div class="wrapper">
  <div class="container">
  <img class="image" src="https://www.inquirer.com/resizer/JVse2HXoMM-7NcrCYLy8QPlLBnY=/800x533/smart/filters:format(webp)/cloudfront-us-east-1.images.arcpublishing.com/pmn/GPCW7HKIGBB35GT5JNSHOYPF7Y.jpeg"/>
  <div class="header">
    <h3>Nicholas Singleton</h3>
    <h4>PSU Football player</h4>
  </div>
  <details class="details">
    <summary>Career Stats</summary>
    <div>
      <ul>
        <li>Big Ten's Freshman of the Year in 2022..</li>
        <li>Penn State running back</li>
       </ul>
    </div>
    </details>
</div>
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
