<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Feliz Cumpleaños 🎂</title>

<style>
*{
  margin:0;
  padding:0;
  box-sizing:border-box;
  font-family: 'Poppins', sans-serif;
}

body{
  height:100vh;
  background: linear-gradient(120deg,#f8b3c8,#d94b4b);
  overflow:hidden;
  color:#fff;
}

/* ===== Globos ===== */
.ballon{
  position:absolute;
  width:60px;
  height:80px;
  border-radius:50%;
  animation: flotar 6s infinite ease-in-out;
  opacity:0.8;
}
.b1{background:#4adede; left:10%; animation-delay:0s;}
.b2{background:#ffd166; right:10%; animation-delay:1s;}
.b3{background:#6aeb6a; bottom:5%; animation-delay:2s;}

@keyframes flotar{
  0%{transform:translateY(0);}
  50%{transform:translateY(-40px);}
  100%{transform:translateY(0);}
}

/* ===== PANTALLA 1 ===== */
.inicio{
  position:absolute;
  inset:0;
  display:flex;
  justify-content:center;
  align-items:center;
}

.card{
  background:rgba(255,255,255,0.25);
  backdrop-filter: blur(10px);
  border-radius:25px;
  padding:30px;
  width:90%;
  max-width:360px;
  text-align:center;
  animation: entrada 1.5s ease forwards;
}

@keyframes entrada{
  from{transform:scale(0.6); opacity:0;}
  to{transform:scale(1); opacity:1;}
}

.card h1{
  font-size:28px;
  margin-bottom:15px;
}

.card p{
  font-size:16px;
  line-height:1.5;
  margin-bottom:20px;
}

button{
  background:#e85d75;
  border:none;
  padding:14px 30px;
  border-radius:40px;
  font-size:16px;
  color:white;
  cursor:pointer;
  animation: latir 1.5s infinite;
}

@keyframes latir{
  0%{transform:scale(1);}
  50%{transform:scale(1.1);}
  100%{transform:scale(1);}
}

/* ===== PANTALLA 2 ===== */
.sorpresa{
  position:absolute;
  inset:0;
  background:linear-gradient(120deg,#ff9a9e,#fad0c4);
  display:flex;
  justify-content:center;
  align-items:center;
  opacity:0;
  pointer-events:none;
  transition:1s;
}

.sorpresa.activa{
  opacity:1;
  pointer-events:auto;
}

/* TARJETA CON SCROLL */
.sorpresa-card{
  background:rgba(0,0,0,0.35);
  border-radius:25px;
  width:90%;
  max-width:420px;
  max-height:85vh;
  overflow-y:auto;
  padding:20px;
  animation: subir 1s ease;
}

@keyframes subir{
  from{transform:translateY(40px); opacity:0;}
  to{transform:translateY(0); opacity:1;}
}

/* Scroll */
.sorpresa-card::-webkit-scrollbar{
  width:6px;
}
.sorpresa-card::-webkit-scrollbar-thumb{
  background:#ff9ecf;
  border-radius:10px;
}

/* IMAGEN (SOLO EN SORPRESA) */
.sorpresa-card img{
  width:100%;
  border-radius:15px;
  margin-bottom:15px;
}

/* TEXTO */
.sorpresa-card h2{
  text-align:center;
  margin-bottom:15px;
}

.sorpresa-card p{
  font-size:15px;
  line-height:1.7;
}

/* Emojis */
.emoji{
  position:absolute;
  font-size:24px;
  animation: subirEmoji 4s infinite linear;
}

@keyframes subirEmoji{
  from{bottom:-40px; opacity:0;}
  to{bottom:110%; opacity:1;}
}
</style>
</head>

<body>

<!-- Globos -->
<div class="ballon b1"></div>
<div class="ballon b2"></div>
<div class="ballon b3"></div>

<!-- INICIO (SIN IMAGEN) -->
<div class="inicio" id="inicio">
  <div class="card">
    <h1>Holaaaaaa wuenosss diasss"conplo"
        🎉 ¡¡¡Feliiiii Cumpleañossss!!! 🎂</h1>
    <p>
      Hoy es un diaa muyyy especial,no?? 💖<br>
      Iraaa hice algo para tiii ✨
    </p>
    <button onclick="mostrar()">🎁 Toca aquí</button>
  </div>
</div>

<!-- SORPRESA (IMAGEN + TEXTO) -->
<div class="sorpresa" id="sorpresa">
  <div class="sorpresa-card">

    <!-- AQUÍ VA LA IMAGEN (DESPUÉS DE PRESIONAR) -->
    <img src="MUS.jpeg" alt="Imagen especial">

    <h2>💖 Para Tiiii 💖</h2>

    <p>
      Hoy es un día muyyyy especial, un dia para celebrar otro añito massss
      ✨quierooo que sepass que eres y siempre seras la niña mas importante para mi y alguien que valoro mushitoo y aprecio profundamente de mi corazonnn💕.<br><br>
      <br><br>
      !!!FELIIIII CUMPLEAÑOS "MI CONPLO✨"  En este dia tan especial me siento muy feliz de celebrarte un añito masss a la niña mas wonita que e conocido
      y la cual se ha vuelto muy especial para miii💖 Te agradezco musho por permitirme estar contigo en este dia tan especial (wueno no en persona pero igual ...me siento muuuuy feliiii)
      quiero desearte un muy wonito diaaa que DIOS te conceda mushisissiisimos añitos mas de vida,salud y que te ayude a cumplir todas tus metas💕<br><br>

      Le doy gracias a Dios por haber encontrado a una niña tan wonita y de buen corazon en estos tiempos de ahora.
    vaya y decir que el año pasado en esta fecha ni sabia de tiii y wuaoo! ahora te has vuelto la personita masss importante para mi ...que cosas del destino,no JSJSAJ
    sabes algo,aparte de mi mamá, TU eres la mujer por la cual doy mi vida. No,no eres mi novia,eres la mujer que deseo tener toda mi vida y apesar
    de mis errores :( nunca dudes que te quiero infinitamente✨🫶🏼 "y pase lo que pase en el futuro...siempreee estare ahii para tiii :)"<br><br>

    Wuenoooo espero que este dia tan especial pala tiii la pases superrrr biennnn y que disfrutes en familia :)
    Te quiero mushisisismo "MI CONPLO✨"...espero que este detallito que hice de corazonnn💕te haya o haiga gustado mushito JSSJSJAJ
    - Masss adelante te dare una jorpresa que tengo para tiii, peroo no te dire cuando JSJSJSJ
<br><br>
    -CON CARIÑO... ALEJANDRO 
    <br><br>PARA :DANIELA ✨💕💕
    </p>

  </div>
</div>

<audio id="musica" src="MUS.mp3"></audio>

<script>
function mostrar(){
  document.getElementById("inicio").style.display="none";
  document.getElementById("sorpresa").classList.add("activa");
  document.getElementById("musica").play();

  for(let i=0;i<20;i++){
    let e=document.createElement("div");
    e.className="emoji";
    e.innerHTML=["💖","✨","🎉","💕","🎂"][Math.floor(Math.random()*5)];
    e.style.left=Math.random()*100+"%";
    e.style.animationDuration=(Math.random()*3+2)+"s";
    document.body.appendChild(e);
  }
}
</script>

</body>
</html>
