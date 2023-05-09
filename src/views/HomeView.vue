<script setup lang="ts">
import IconCommunity from '@/components/icons/IconCommunity.vue';
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
 nav{
  
 }

 h1{
  margin: 20px;
  margin-left: 30px;
  font-size: 30px;
  cursor: pointer;
 }

 ul{
  list-style-type: none;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0;
 }
 .main-nav{
  display: flex;
  justify-content: center;
  padding: 0
 }
 li{
  font-size: 20px;
  font-weight: 600;
  margin: 15px 25px 15px 25px;
  cursor: pointer;
 }
 li:hover::after{
  content: ;
 }
 button{
  margin: 20px;
  margin-right: 30px;
  border: none;
  color: #333;
  background-color: #E5EAF5;
  padding: 10px 20px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  border-radius: 12px;
  cursor: pointer;
  filter: drop-shadow(3px 5px 2px #333);
 }
</style>