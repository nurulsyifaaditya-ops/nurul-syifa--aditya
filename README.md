<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Ajakan Berenang</title>

  <style>
    *{
      margin:0;
      padding:0;
      box-sizing:border-box;
      font-family: Arial, Helvetica, sans-serif;
    }

    body{
      height:100vh;
      overflow:hidden;
      display:flex;
      justify-content:center;
      align-items:center;
      background: linear-gradient(135deg, #4da6ff, #ffffff, #ffb347);
    }

    .container{
      width:90%;
      max-width:700px;
      background:white;
      border-radius:25px;
      padding:40px;
      text-align:center;
      box-shadow:0 10px 30px rgba(0,0,0,0.2);
      position:relative;
      border:5px solid #4da6ff;
    }

    h1{
      color:#0077ff;
      margin-bottom:15px;
      font-size:38px;
    }

    p{
      color:#444;
      font-size:18px;
      margin-bottom:25px;
      line-height:1.7;
    }

    .stickers{
      font-size:55px;
      margin-bottom:20px;
      animation: float 2s infinite ease-in-out;
    }

    @keyframes float{
      0%{ transform: translateY(0px);}
      50%{ transform: translateY(-10px);}
      100%{ transform: translateY(0px);}
    }

    .buttons{
      position:relative;
      height:130px;
    }

    button{
      padding:15px 35px;
      border:none;
      border-radius:15px;
      font-size:18px;
      cursor:pointer;
      transition:0.3s;
      font-weight:bold;
    }

    #yesBtn{
      background:#ff9f1c;
      color:white;
      margin-right:20px;
    }

    #yesBtn:hover{
      background:#ff8500;
      transform:scale(1.08);
    }

    #noBtn{
      background:#3399ff;
      color:white;
      position:absolute;
    }

    #message{
      margin-top:25px;
      font-size:22px;
      color:#ff8500;
      font-weight:bold;
      display:none;
      animation: fade 0.5s ease;
      line-height:1.8;
    }

    @keyframes fade{
      from{
        opacity:0;
        transform:translateY(10px);
      }
      to{
        opacity:1;
        transform:translateY(0);
      }
    }

    .benefit{
      margin-top:25px;
      background:#eaf5ff;
      padding:20px;
      border-radius:15px;
      text-align:left;
    }

    .benefit h3{
      color:#0077ff;
      margin-bottom:10px;
    }

    .benefit ul{
      padding-left:20px;
      line-height:1.8;
      color:#444;
    }

  </style>
</head>

<body>

  <div class="container">

    <div class="stickers">
      🏊 🌊 ☀️ 🐬 💪
    </div>

    <h1>Ayo Berenang!</h1>

    <p>
      Berenang adalah olahraga yang menyenangkan dan menyehatkan.
      Selain membuat tubuh segar, berenang juga membantu melatih postur tubuh,
      menjaga kesehatan, dan mendukung pertumbuhan tubuh agar lebih optimal!
    </p>

    <div class="buttons">
      <button id="yesBtn">Iya Mau Berenang 🏊</button>
      <button id="noBtn">Tidak 😅</button>
    </div>

    <div id="message">
      Hebat! 🌊✨<br><br>
      Dengan rutin berenang:
      <br><br>
      💪 Tubuh jadi lebih sehat<br>
      📏 Postur tubuh lebih baik<br>
      😄 Pikiran lebih segar<br>
      🏊 Badan lebih aktif dan kuat<br><br>
      Semangat olahraga dan jaga kesehatan ya! ☀️
    </div>

    <div class="benefit">
      <h3>Manfaat Berenang:</h3>
      <ul>
        <li>Melatih seluruh otot tubuh</li>
        <li>Meningkatkan stamina dan pernapasan</li>
        <li>Membantu menjaga postur tubuh</li>
        <li>Membuat tubuh lebih bugar dan aktif</li>
      </ul>
    </div>

  </div>

  <script>
    const noBtn = document.getElementById("noBtn");
    const yesBtn = document.getElementById("yesBtn");
    const message = document.getElement
