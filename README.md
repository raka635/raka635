
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>ORBIT AI | Discover New Possibilities</title>
<style>
* { box-sizing: border-box; }
body {
  margin: 0;
  font-family: Arial, sans-serif;
  background: #080d1c;
  color: white;
}
header {
  padding: 24px 8%;
  display: flex;
  justify-content: space-between;
  align-items: center;
  border-bottom: 1px solid #202b46;
}
.logo { font-size: 27px; font-weight: bold; color: #a78bfa; }
nav a { color: #ddd; margin-left: 20px; text-decoration: none; }
.hero {
  text-align: center;
  padding: 100px 20px;
  background: radial-gradient(circle, #25205a, #080d1c 65%);
}
.hero h1 { font-size: clamp(42px, 8vw, 76px); margin: 10px; }
.hero h1 span { color: #a78bfa; }
.hero p { color: #c4c9da; font-size: 18px; line-height: 1.7; }
.button {
  display: inline-block;
  background: #8059e8;
  color: white;
  padding: 15px 25px;
  border-radius: 10px;
  text-decoration: none;
  margin-top: 20px;
}
section { padding: 65px 9%; text-align: center; }
.cards {
  display: grid;
  grid-template-columns: repeat(auto-fit,minmax(210px,1fr));
  gap: 20px;
  margin-top: 30px;
}
.card {
  background: #111a31;
  border: 1px solid #293654;
  border-radius: 15px;
  padding: 25px;
}
.card h3 { color: #b69aff; }
.card p { color: #c4c9da; line-height: 1.6; }
textarea {
  width: 100%;
  max-width: 600px;
  min-height: 120px;
  padding: 15px;
  border-radius: 10px;
  background: #111a31;
  color: white;
  border: 1px solid #53618b;
  font: inherit;
}
footer {
  text-align: center;
  padding: 30px;
  color: #9ca3b8;
  border-top: 1px solid #202b46;
}
</style>
</head>
<body>
<header>
  <div class="logo">✧ ORBIT</div>
  <nav><a href="#mission">Mission</a><a href="#features">Features</a><a href="#lab">Discovery Lab</a></nav>
</header>

<div class="hero">
  <div style="font-size:65px">🌌</div>
  <h1>Think Beyond.<br><span>Discover More.</span></h1>
  <p>Welcome to ORBIT — an experimental AI discovery project<br>
  designed to explore difficult problems and imagine new solutions.</p>
  <a class="button" href="#lab">Explore Discovery Lab</a>
</div>

<section id="mission">
  <h2>Our Mission</h2>
  <p>Help humanity investigate difficult problems, connect ideas<br>
  and discover possibilities that have not yet been explored.</p>
</section>

<section id="features">
  <h2>ORBIT Intelligence</h2>
  <div class="cards">
    <div class="card"><h3>🧠 Problem Detective</h3><p>Investigate root causes and hidden assumptions.</p></div>
    <div class="card"><h3>💡 Possibility Engine</h3><p>Generate creative approaches to challenging problems.</p></div>
    <div class="card"><h3>🔬 Reality Checker</h3><p>Separate evidence from ideas and hypotheses.</p></div>
    <div class="card"><h3>🚀 Discovery Memory</h3><p>Learn from experiments and previous discoveries.</p></div>
  </div>
</section>

<section id="lab">
  <h2>ORBIT Discovery Lab</h2>
  <p>What problem would you like to investigate?</p>
  <textarea id="problem" placeholder="Describe your problem here..."></textarea><br>
  <button class="button" onclick="investigate()">Explore this idea</button>
  <p id="result" aria-live="polite"></p>
</section>

<footer>
  © 2026 ORBIT AI Project · Exploring New Possibilities
</footer>

<script>
function investigate() {
  const problem = document.getElementById("problem").value.trim();
  const result = document.getElementById("result");
  if (!problem) {
    result.textContent = "Please describe a problem first.";
    return;
  }
  result.textContent =
    "Your investigation topic: " + problem +
    ". ORBIT's next step is to research existing knowledge, identify gaps and develop testable ideas.";
}
</script>
</body>
</html>
