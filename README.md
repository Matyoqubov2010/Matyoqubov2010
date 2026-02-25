![511691400-55711378-b70b-4895-a1e3-f7f75a512312](https://github.com/user-attachments/assets/c4f49e62-3e23-476a-9b3d-7b49aba0911c)
<img width="2000" height="400" alt="511691580-d1268492-1814-4d0c-9383-f17e0260f10f" src="https://github.com/user-attachments/assets/5017e395-7ce9-4363-9668-cce13049ff69" />

  ![Typing Text](https://readme-typing-svg.demolab.com?lines=Salom!+Men+ismim+Matyoqubov+Umidbek+Umirbek+ogli.;IT+sohasiga+qiziqaman+maqsadim+web+dasturchi+bo'lish.&font=Fira+Code&size=25&pause=1000&color=0000FF&center=true&vCenter=true&width=1200)
 
<h1> Hi there I`m Matyoqubov2010👋</h1>
<h2>Mening IT ko`nikmalarim</h2>
<ol>
 <li>HTML</li>
 <li>CSS</li>
 <li>JAVASCRIPT</li>
 <li>Python</li>
</ol>

<!DOCTYPE html>
<html lang="uz">
<head>
<meta charset="UTF-8">
<title>Pacman Game</title>
<style>
  body{
    margin:0;
    background:black;
    display:flex;
    justify-content:center;
    align-items:center;
    height:100vh;
  }
  canvas{
    background:#111;
  }
</style>
</head>
<body>

<canvas id="game" width="400" height="400"></canvas>

<script>
const canvas = document.getElementById("game");
const ctx = canvas.getContext("2d");

let pacman = {
  x: 200,
  y: 200,
  r: 20,
  dx: 0,
  dy: 0
};

document.addEventListener("keydown", e=>{
  if(e.key==="ArrowRight"){pacman.dx=3; pacman.dy=0;}
  if(e.key==="ArrowLeft"){pacman.dx=-3; pacman.dy=0;}
  if(e.key==="ArrowUp"){pacman.dy=-3; pacman.dx=0;}
  if(e.key==="ArrowDown"){pacman.dy=3; pacman.dx=0;}
});

function drawPacman(){
  ctx.beginPath();
  ctx.arc(pacman.x, pacman.y, pacman.r, 0.2*Math.PI, 1.8*Math.PI);
  ctx.lineTo(pacman.x, pacman.y);
  ctx.fillStyle="yellow";
  ctx.fill();
}

function update(){
  ctx.clearRect(0,0,400,400);

  pacman.x += pacman.dx;
  pacman.y += pacman.dy;

  drawPacman();

  requestAnimationFrame(update);
}

update();
</script>

</body>
</html>
<!--
**Matyoqubov2010/Matyoqubov2010** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
