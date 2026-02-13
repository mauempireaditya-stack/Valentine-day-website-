# Valentine-day-website-
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Will You Be My Valentine? ❤️</title>

<style>
body {
    margin: 0;
    font-family: 'Segoe UI', sans-serif;
    background: linear-gradient(135deg, #ff9a9e, #fad0c4);
    overflow: hidden;
    text-align: center;
}

.container {
    position: relative;
    top: 20vh;
}

h1 {
    font-size: 3em;
    color: white;
    text-shadow: 2px 2px 10px rgba(0,0,0,0.2);
    animation: fadeIn 2s ease-in-out;
}

.buttons {
    margin-top: 30px;
}

button {
    padding: 15px 30px;
    font-size: 18px;
    border: none;
    border-radius: 30px;
    cursor: pointer;
    margin: 10px;
    transition: 0.3s;
}

.yes {
    background: #ff4e8a;
    color: white;
}

.no {
    background: #ffffff;
    color: #ff4e8a;
}

button:hover {
    transform: scale(1.1);
}

.polaroid {
    display: none;
    margin-top: 40px;
    background: white;
    padding: 15px;
    width: 250px;
    margin-left: auto;
    margin-right: auto;
    box-shadow: 0 10px 20px rgba(0,0,0,0.2);
    transform: rotate(-3deg);
}

.polaroid img {
    width: 100%;
    height: auto;
}

.caption {
    margin-top: 10px;
    font-style: italic;
    color: #444;
}

@keyframes fadeIn {
    from {opacity: 0;}
    to {opacity: 1;}
}
</style>
</head>

<body>

<div class="container">
    <h1>Will You Be My Valentine? 💖</h1>

    <div class="buttons">
        <button class="yes" onclick="showLove()">Of Course Yes 😍</button>
        <button class="no" onmouseover="moveButton(this)">Absolutely No 😜</button>
    </div>

    <div class="polaroid" id="loveBox">
        <img src="herphoto.jpg" alt="Her Photo">
        <div class="caption">
            "From the moment I met you, everything felt brighter.  
            You make my world beautiful. ❤️"
        </div>
    </div>
</div>

<script>
function showLove() {
    document.getElementById("loveBox").style.display = "block";
}

function moveButton(btn) {
    btn.style.position = "absolute";
    btn.style.top = Math.random() * window.innerHeight + "px";
    btn.style.left = Math.random() * window.innerWidth + "px";
}
</script>

</body>
</html>
