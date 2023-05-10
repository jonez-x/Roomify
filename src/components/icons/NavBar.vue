<script setup lang="ts">
</script>

<template>
    <nav>
      <ul>
        <h1>Roomify</h1>
        <div class="main-nav">
          <li><a>Home </a></li>
          <li><a>Scene Editor</a></li>
          <li><a>Settings</a></li>
        </div>
         <button>Log in</button>
      </ul>
    </nav>
</template>

<style scoped>
 h1{
  margin: 20px;
  margin-left: 30px;
  font-size: 30px;
  cursor: pointer;
  color: #FF4500;
  user-select: none;
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
 a{
  user-select: none;
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
  background-color: #FF4500;
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