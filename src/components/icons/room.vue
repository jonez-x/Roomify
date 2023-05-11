<script  lang="ts">
import * as THREE from 'three';
import { onMounted } from 'vue';

const scene = new THREE.Scene();
scene.background = new THREE.Color( 0x191414);
const camera = new THREE.PerspectiveCamera( 100, (window.innerWidth/3) / (window.innerHeight/3), 0.1, 1000 );
const renderer = new THREE.WebGLRenderer();
renderer.setSize( window.innerWidth, window.innerHeight );

export default {
  mounted() {
    this.$refs.scene.appendChild( renderer.domElement );
  }
}

const geometry = new THREE.BoxGeometry( 1, 1, 1 );
const material = new THREE.MeshBasicMaterial( { color:  0x1e90ff} );
const cube = new THREE.Mesh( geometry, material );
scene.add( cube );

camera.position.z = 1.5;

function animate() {
	requestAnimationFrame( animate );

	cube.rotation.x += 0.01;
	cube.rotation.y += 0.01;

	renderer.render( scene, camera );
}

animate();
</script>

<template>
   <div ref="scene">
   </div>
</template>

<style scoped>
</style>