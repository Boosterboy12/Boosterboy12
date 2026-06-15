<!-- ========================= -->
<!--  VIHAAN THE LEGEND README -->
<!-- ========================= -->

<div align="center">

# 🌌 VIHAAN | The Legend

<img src="https://readme-typing-svg.herokuapp.com?font=Orbitron&size=28&duration=3000&pause=500&color=00F5FF&center=true&vCenter=true&width=800&lines=Full-Stack+Developer;AI+Explorer;3D+Experience+Builder;Future+Architect" />

<br/>

<!-- 3D HERO VISUAL (Embedded Scene Placeholder) -->
<a href="https://threejs.org/">
  <img src="https://raw.githubusercontent.com/mrdoob/three.js/dev/examples/screenshots/interactive_cubes.jpg" width="90%" />
</a>

<p>
⚡ A next-gen interactive GitHub profile blending <b>3D visuals</b>, <b>AI systems</b>, and <b>futuristic UI design</b> ⚡
</p>

</div>

---

## 🌐 3D Interactive Experience (Live Scene)

> 🧠 This README integrates a **Three.js-powered 3D universe** (hosted externally due to GitHub limitations).

### 🚀 Launch 3D Scene
👉 Click here to explore:  
**https://YOUR-3D-DEMO-LINK.vercel.app**

---

### 🧊 Embedded Concept (Three.js Skeleton)

```html
<!-- ⚠️ GitHub doesn't fully execute JS in README, so this is for external hosting only -->

<script type="module">
import * as THREE from "https://cdn.jsdelivr.net/npm/three@0.160/build/three.module.js";

const scene = new THREE.Scene();
const camera = new THREE.PerspectiveCamera(75, window.innerWidth/window.innerHeight, 0.1, 1000);

const renderer = new THREE.WebGLRenderer({ antialias: true });
renderer.setSize(window.innerWidth, window.innerHeight);
document.body.appendChild(renderer.domElement);

// 3D Cube
const geometry = new THREE.BoxGeometry();
const material = new THREE.MeshStandardMaterial({ color: 0x00f5ff, wireframe: true });
const cube = new THREE.Mesh(geometry, material);
scene.add(cube);

// Light
const light = new THREE.PointLight(0xffffff, 1);
light.position.set(5,5,5);
scene.add(light);

camera.position.z = 3;

function animate(){
  requestAnimationFrame(animate);
  cube.rotation.x += 0.01;
  cube.rotation.y += 0.01;
  renderer.render(scene, camera);
}
animate();
</script>
