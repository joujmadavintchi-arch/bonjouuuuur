<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<title>Bonjouuuurattttt 3inaya 🌹</title>
<style>
  body {
    margin: 0;
    overflow: hidden;
    background: linear-gradient(to top, #ffdde1, #ee9ca7);
    height: 100vh;
  }
  .rose {
    position: absolute;
    width: 40px;
    height: 40px;
    background-image: url('https://pngimg.com/uploads/rose/rose_PNG667.png');
    background-size: cover;
    animation: fall 5s linear forwards;
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
    transition: opacity 2s ease;
  }
</style>
</head>
<body>
<script>
  // توليد ورود عشوائية
  for (let i = 0; i < 25; i++) {
    const rose = document.createElement('div');
    rose.className = 'rose';
    rose.style.left = Math.random() * window.innerWidth + 'px';
    rose.style.animationDelay = Math.random() * 3 + 's';
    document.body.appendChild(rose);
  }

  // إظهار النص بعد 5 ثواني
  setTimeout(() => {
    document.querySelector('.text').style.opacity = 1;
  }, 5000);
</script>
<div class="text">bonjouuuurattttt 3inaya 🌹</div>
</body>
</html>