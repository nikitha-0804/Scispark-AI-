# Scispark-AI-
Scispark-AI - wonder science discover world
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>SciSpark AI</title>

<style>
body {
  margin: 0;
  font-family: Arial, sans-serif;
  background: #071426;
  color: white;
  text-align: center;
}

header {
  background: #102b46;
  padding: 25px;
}

h1 {
  color: #38e8c6;
  font-size: 36px;
}

main {
  padding: 20px;
}

.card {
  background: #142b42;
  padding: 22px;
  margin: 18px auto;
  border-radius: 16px;
  max-width: 420px;
}

button {
  background: #38e8c6;
  color: #071426;
  padding: 12px 20px;
  border: none;
  border-radius: 10px;
  font-weight: bold;
  cursor: pointer;
}

input {
  box-sizing: border-box;
  width: 100%;
  padding: 12px;
  margin-bottom: 12px;
  border-radius: 8px;
  border: none;
}

footer {
  padding: 20px;
  color: #b8c7d9;
}
</style>
</head>

<body>

<header>
  <h1>🧬 SciSpark AI</h1>
  <p>Explore Science. Discover Wonders. Spark Genius!</p>
</header>

<main>

  <div class="card">
    <h2>🧠 AI Science Tutor</h2>
    <p>Enter a science question to create a study prompt.</p>
    <input id="question"
      placeholder="Ask a science question...">
    <button onclick="askScience()">Explore</button>
    <p id="answer"></p>
  </div>

  <div class="card">
    <h2>🔬 Science Genius Quiz</h2>
    <p>Which planet is known as the Red Planet?</p>
    <button onclick="checkAnswer('Earth')">Earth</button>
    <button onclick="checkAnswer('Mars')">Mars</button>
    <button onclick="checkAnswer('Venus')">Venus</button>
    <p id="quiz"></p>
  </div>

  <div class="card">
    <h2>🌱 Science Explorer</h2>
    <p>Plants use sunlight, water and carbon dioxide
    to make their food through photosynthesis.</p>
    <button onclick="showFact()">Discover a Fact</button>
    <p id="fact"></p>
  </div>

</main>

<footer>
  <p>✨ Keep Exploring with SciSpark AI ✨</p>
</footer>

<script>
function askScience() {
  const q = document.getElementById("question").value.trim();

  document.getElementById("answer").textContent =
    q ? "Study prompt: Explain " + q +
    " in simple words, give an example, and provide 3 quiz questions."
    : "Please enter a science question!";
}

function checkAnswer(answer) {
  document.getElementById("quiz").textContent =
    answer === "Mars"
    ? "🎉 Correct! Mars is the Red Planet!"
    : "Try again! Think about the Red Planet.";
}

function showFact() {
  document.getElementById("fact").textContent =
    "🌿 Plants capture sunlight using chlorophyll!";
}
</script>

</body>
</html>
