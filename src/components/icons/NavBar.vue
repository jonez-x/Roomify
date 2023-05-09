<script setup lang="ts">
</script>

<template>
  <main>
    <nav>
      <ul>
        <h1>Roomify</h1>
        <div class="main-nav">
          <li><a>Home </a><v-icon icon="mdi-vuetify"></v-icon></li>
          <li><a>Scene Editor</a></li>
          <li><a>Settings</a></li>
        </div>
         <button>Log in</button>
      </ul>
    </nav>
  </main>
</template>

<style>
 h1{
  margin: 20px;
  margin-left: 30px;
  font-size: 30px;
  cursor: pointer;
  color: #1DB954;
 }

 ul{
  list-style-type: none;
  display: flex;
  align-items: flex-start;
  justify-content: space-between;
  padding: 0;
 }
 .main-nav{
  display: flex;
  justify-content: center;
  margin-right: 13px;
 }
 li{
  font-size: 20px;
  font-weight: 600;
  margin: 15px 25px 15px 25px;
  cursor: pointer;
  padding: 20px;
 }
 li:hover{
  transition: ease-in-out 150ms;
  transform: translateY(-10px);
 }
 li:not(:hover){
   transition: ease-in-out 150ms;
   transform: translateY(0);
 }
 button{
  margin: 20px;
  margin-right: 30px;
  border: none;
  color: #191414;
  font-family: Montserrat;
  font-weight: 600;
  background-color: #1DB954;
  padding: 10px 20px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  border-radius: 12px;
  cursor: pointer;
  filter: drop-shadow(3px 5px 2px #111111);
 }
</style>