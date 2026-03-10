<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>For My Love</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    body {
      margin: 0;
      font-family: 'Arial', sans-serif;
      background: linear-gradient(270deg, #ff9a9e, #fad0c4, #fbc2eb, #a6c1ee);
      background-size: 800% 800%;
      animation: gradientBG 15s ease infinite;
      overflow: hidden;
      text-align: center;
      color: #fff;
    }
    .slide {
      display: none;
      height: 100vh;
      justify-content: center;
      align-items: center;
      flex-direction: column;
      padding: 20px;
    }
    .active {
      display: flex;
      animation: fadeIn 2s ease-in-out;
    }
    h1 {
      font-size: 2.5em;
      animation: glow 2s infinite alternate, bounce 3s infinite;
    }
    p {
      font-size: 1.2em;
      margin-top: 20px;
      animation: slideUp 2s ease-in-out;
    }
    input, button {
      padding: 12px;
      font-size: 1.2em;
      border-radius: 10px;
      border: none;
      text-align: center;
      animation: pulse 2s infinite;
      width: 80%;
      max-width: 300px;
    }
    button {
      margin-top: 20px;
      background: #d6336c;
      color: white;
      cursor: pointer;
    }
    @keyframes fadeIn { from {opacity: 0;} to {opacity: 1;} }
    @keyframes slideUp { from {transform: translateY(50px); opacity: 0;} to {transform: translateY(0); opacity: 1;} }
    @keyframes glow { from {text-shadow: 0 0 10px #ff6b6b;} to {text-shadow: 0 0 30px #ff0000;} }
    @keyframes pulse { 0% {transform: scale(1);} 50% {transform: scale(1.1);} 100% {transform: scale(1);} }
    @keyframes bounce { 0%,100% {transform: translateY(0);} 50% {transform: translateY(-15px);} }
    @keyframes gradientBG { 0% {background-position:0% 50%;} 50% {background-position:100% 50%;} 100% {background-position:0% 50%;} }
    .heart {
      position: absolute;
      color: red;
      font-size: 2em;
      animation: floatUp 6s infinite;
    }
    @keyframes floatUp {
      0% {transform: translateY(100vh) scale(0.5); opacity: 0;}
      50% {opacity: 1;}
      100% {transform: translateY(-10vh) scale(1.2); opacity: 0;}
    }
  </style>
</head>
<body>
  <!-- Slide 1 -->
  <div id="slide1" class="slide active">
    <h1>Enter Your Name 💕</h1>
    <input type="text" id="nameInput" placeholder="Your Name">
    <button onclick="showLove()">Continue</button>
  </div>
  <!-- Slide 2 -->
  <div id="slide2" class="slide">
    <h1 id="loveMessage"></h1>
    <p>You are my forever ✨</p>
  </div>
  <script>
    function showLove() {
      const name = document.getElementById("nameInput").value;
      document.getElementById("slide1").classList.remove("active");
      document.getElementById("slide2").classList.add("active");
      document.getElementById("loveMessage").innerHTML = "I Love You, " + name + " ❤️";
    }
    function createHeart() {
      const heart = document.createElement("div");
      heart.className = "heart";
      heart.innerHTML = "❤";
      heart.style.left = Math.random() * window.innerWidth + "px";
      document.body.appendChild(heart);
      setTimeout(() => heart.remove(), 6000);
    }
    setInterval(createHeart, 800);
  </script>
</body>
</html>
