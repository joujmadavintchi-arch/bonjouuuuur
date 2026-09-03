<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<title>Bonjouuuurattttt 3inaya 🌹</title>
<style>
  body {
    margin: 0;
    overflow: hidden;
    background: linear-gradient(to top, #ffb6c1, #ffe4e1);
    height: 100vh;
  }
  .rose {
    position: absolute;
    width: 40px;
    height: 40px;
    background-image: url('https://pngimg.com/uploads/rose/rose_PNG667.png');
    background-size: cover;
    animation: fall 5s linear infinite;
  }
  @keyframes fall {
    0% { transform: translateY(-50px) rotate(0deg); opacity: 1; }
    100% { transform: translateY(100vh) rotate(360deg); opacity: 0; }
  }
  .text {
    position: absolute;
    top: 45%;
    width: 100%;
    text-align: center;
    font-size: 3em;
    font-family: 'Cairo', sans-serif;
    color: #b30059;
    opacity: 0;
    animation: showText 2s ease forwards;
    animation-delay: 5s;
  }
  @keyframes showText {
    to { opacity: 1; transform: scale(1.1); }
  }
</style>
</head>
<body>
<script>
  for (let i = 0; i < 30; i++) {
    const rose = document.createElement('div');
    rose.className = 'rose';
    rose.style.left = Math.random() * window.innerWidth + 'px';
    rose.style.animationDelay = Math.random() * 5 + 's';
    document.body.appendChild(rose);
  }
</script>
<div class="text">bonjouuuurattttt 3inaya 🌹</div>
</body>
</html># bonjouuuuur