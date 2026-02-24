<!DOCTYPE html>
<html lang="ja">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>My Portfolio</title>

<style>
body {
  margin: 0;
  font-family: Arial, sans-serif;
  transition: 0.3s;
}

/* ヘッダー */
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 20px;
  background: #222;
  color: white;
}

button {
  padding: 8px 15px;
  cursor: pointer;
  border: none;
  border-radius: 5px;
}

/* ヒーロー */
.hero {
  text-align: center;
  padding: 100px 20px;
  background: linear-gradient(135deg, #667eea, #764ba2);
  color: white;
}

/* 作品 */
.works {
  padding: 60px 20px;
  text-align: center;
}

.card {
  display: inline-block;
  width: 250px;
  padding: 20px;
  margin: 15px;
  background: white;
  border-radius: 12px;
  box-shadow: 0 5px 15px rgba(0,0,0,0.1);
  transition: 0.3s;
  opacity: 0;
  transform: translateY(40px);
}

.card:hover {
  transform: translateY(-10px);
}

/* スキル */
.skills {
  padding: 60px 20px;
  background: #f4f4f4;
  text-align: center;
}

/* ダークモード */
.dark {
  background: #111;
  color: white;
}

.dark header {
  background: black;
}

.dark .skills {
  background: #222;
}

.dark .card {
  background: #333;
  color: white;
}
</style>

</head>
<body>

<header>
  <h1>My Portfolio</h1>
  <button id="darkBtn">🌙 Dark</button>
</header>

<section class="hero">
  <h2>Web Developer</h2>
  <p>HTML / CSS / JavaScript</p>
</section>

<section class="works">
  <h2>Works</h2>
  <div class="card">LP制作</div>
  <div class="card">TODOリスト</div>
  <div class="card">ポートフォリオ</div>
</section>

<section class="skills">
  <h2>Skills</h2>
  <p>HTML ★★★★☆</p>
  <p>CSS ★★★★☆</p>
  <p>JavaScript ★★★☆☆</p>
</section>

<script>
// ダークモード
const btn = document.getElementById("darkBtn");

btn.addEventListener("click", () => {
  document.body.classList.toggle("dark");
});

// スクロールアニメーション
const cards = document.querySelectorAll(".card");

window.addEventListener("scroll", () => {
  cards.forEach(card => {
    const position = card.getBoundingClientRect().top;
    const screenPosition = window.innerHeight / 1.2;

    if (position < screenPosition) {
      card.style.opacity = "1";
      card.style.transform = "translateY(0)";
    }
  });
});
</script>

</body>
</html>
