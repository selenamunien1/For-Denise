# For-Denise
For my love
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>My Answered Prayer ❤️</title>

<style>
body {
    margin: 0;
    font-family: 'Segoe UI', sans-serif;
    background: linear-gradient(to right, #2b1a12, #8b5e3c);
    color: white;
    text-align: center;
    overflow-x: hidden;
}

.heart {
    position: fixed;
    bottom: -10px;
    animation: floatUp 6s linear infinite;
}

@keyframes floatUp {
    0% { transform: translateY(0); opacity: 1; }
    100% { transform: translateY(-100vh); opacity: 0; }
}

.container {
    padding: 40px 20px;
}

h1 {
    font-size: 2.5em;
}

img {
    width: 260px;
    border-radius: 20px;
    margin: 20px 0;
    box-shadow: 0 10px 30px rgba(0,0,0,0.5);
}

.button {
    padding: 12px 25px;
    background: #d4a373;
    border-radius: 25px;
    border: none;
    color: white;
    font-size: 16px;
    cursor: pointer;
}

.button:hover {
    background: #c0895b;
}

.hidden {
    display: none;
    margin-top: 20px;
    font-size: 1.2em;
}

.gallery img {
    width: 140px;
    margin: 8px;
    border-radius: 10px;
}

.countdown {
    font-size: 1.3em;
    margin-top: 20px;
}

footer {
    margin-top: 50px;
    opacity: 0.7;
}
</style>
</head>

<body>

<div class="container">

<h1>To My Answered Prayer ❤️</h1>

<img src="your-photo.jpg" alt="My Love">

<p>
From the moment you came into my life, everything started making sense.<br><br>
You are my peace in chaos, my joy in every moment, and the love I never knew I needed so deeply.<br><br>
You didn’t just come into my life… you changed it completely.<br><br>
I thank God for you every single day because you are truly my answered prayer 💖
</p>

<button class="button" onclick="showMessage()">Tap here my love 😊</button>

<div id="message" class="hidden">
    I will choose you again and again… in every lifetime ❤️
</div>

<div class="countdown" id="countdown"></div>

<h2>Our Beautiful Memories 📸</h2>
<div class="gallery">
    <img src="photo1.jpg">
    <img src="photo2.jpg">
    <img src="photo3.jpg">
</div>

<br>

<audio controls autoplay loop>
    <source src="song.mp3" type="audio/mpeg">
</audio>

<br><br>

<a href="https://wa.me/?text=I%20love%20you%20so%20much%20my%20answered%20prayer%20❤️" target="_blank">
    <button class="button">Send You Love 💬</button>
</a>

<footer>
Made with endless love by Selena ❤️
</footer>

</div>

<script>
function showMessage() {
    document.getElementById("message").style.display = "block";
}

// Floating hearts
setInterval(() => {
    let heart = document.createElement("div");
    heart.className = "heart";
    heart.innerHTML = "❤️";
    heart.style.left = Math.random() * 100 + "vw";
    heart.style.fontSize = Math.random() * 20 + 10 + "px";
    document.body.appendChild(heart);
    setTimeout(() => heart.remove(), 6000);
}, 500);

// Countdown (you can change this date later)
let targetDate = new Date("Dec 31, 2026 00:00:00").getTime();

setInterval(function() {
    let now = new Date().getTime();
    let distance = targetDate - now;

    let days = Math.floor(distance / (1000 * 60 * 60 * 24));
    let hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));

    document.getElementById("countdown").innerHTML =
    "Counting down to more beautiful memories ❤️: " + days + " days " + hours + " hours";
}, 1000);
</script>

</body>
</html>