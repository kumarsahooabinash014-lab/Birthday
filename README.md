<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Happy Birthday My Pookie Princess 💖</title>
<style>
    body {
        margin: 0;
        padding: 0;
        background: linear-gradient(135deg, #ffe6f0, #ffffff);
        font-family: "Poppins", sans-serif;
        color: #ff4d94;
        text-align: center;
        /* removed overflow:hidden to allow scrolling */
    }

    .container {
        position: relative;
        z-index: 2;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        padding: 20px;
        animation: fadeIn 2s ease-in;
    }

    img {
        width: 300px;
        max-width: 90%;
        border-radius: 20px;
        box-shadow: 0 0 30px rgba(255, 182, 193, 0.7);
        margin-bottom: 20px;
        animation: float 4s ease-in-out infinite;
    }

    h1 {
        font-size: 2.5em;
        margin: 10px 0;
        text-shadow: 0 0 15px rgba(255,105,180,0.4);
        animation: glow 2s ease-in-out infinite alternate;
    }

    p {
        font-size: 1.1em;
        max-width: 650px;
        background: rgba(255, 255, 255, 0.7);
        padding: 20px;
        border-radius: 25px;
        line-height: 1.6;
        box-shadow: 0 0 15px rgba(255, 192, 203, 0.5);
        animation: fadeIn 3s ease-in;
        margin-bottom: 50px;
    }

    @keyframes fadeIn {
        from {opacity: 0; transform: translateY(30px);}
        to {opacity: 1; transform: translateY(0);}
    }

    @keyframes glow {
        from {text-shadow: 0 0 10px #ff99c8;}
        to {text-shadow: 0 0 25px #ff4d94;}
    }

    @keyframes float {
        0%, 100% {transform: translateY(0);}
        50% {transform: translateY(-10px);}
    }

    /* Confetti */
    .confetti {
        position: fixed; /* stay on screen while scrolling */
        width: 10px;
        height: 10px;
        top: -10px;
        border-radius: 50%;
        animation: fall linear infinite;
        opacity: 0.8;
        z-index: 1;
    }

    @keyframes fall {
        0% {transform: translateY(-10px) rotate(0deg);}
        100% {transform: translateY(110vh) rotate(360deg);}
    }

    /* Floating hearts */
    .heart {
        position: fixed; /* stay on screen while scrolling */
        bottom: -10px;
        color: #ff80aa;
        font-size: 20px;
        animation: rise 6s linear infinite;
        opacity: 0.8;
        z-index: 1;
    }

    @keyframes rise {
        0% {transform: translateY(0) scale(1);}
        100% {transform: translateY(-110vh) scale(1.5); opacity: 0;}
    }
</style>
</head>
<body>

<div class="container">
    <img src="https://i.postimg.cc/LXYCYPNW/Screenshot-20251012-172442-Instagram.jpg" alt="Cute Couple Image">
    <h1>Happy Birthdayy 🥳,<br>my Pookie Princess 🤭💗</h1>
    <p>
        My Favourite Person 🫶<br><br>
        It’s crazy how someone miles away feels so close to me every single day.  
        You’ve got this way of making my mood lighter, my day warmer ☁️ and my heart calm without even trying 🌸.<br><br>
        I don’t even know how you do it, but I swear I’m so glad it’s you 👉👈❤️💫.<br><br>
        You’re not just “someone I talk to,” you’re honestly my comfort zone now — my person. 💖<br><br>
        I hope today gives you every bit of happiness you deserve (and maybe a little extra from me 😌).  
        Just know that even from miles away, I’m always cheering for your smile 🤍<br><br>
        Happy Birthday again, My Amen🌙💫
    </p>
</div>

<audio autoplay loop>
  <p>🎵 Listen to your birthday song <a href="https://spotify.link/SK6lBu6yyXb" target="_blank">here</a>!</p>
    Your browser does not support the audio element.
</audio>

<script>
    // Confetti
    for(let i = 0; i < 100; i++) {
        const c = document.createElement('div');
        c.classList.add('confetti');
        c.style.left = Math.random() * 100 + 'vw';
        c.style.backgroundColor = `hsl(${Math.random()*360}, 70%, 75%)`;
        c.style.animationDuration = (3 + Math.random() * 4) + 's';
        document.body.appendChild(c);
    }

    // Floating hearts
    const hearts = ["💗","💖","💕","💞","💘"];
    setInterval(() => {
        const h = document.createElement("div");
        h.className = "heart";
        h.textContent = hearts[Math.floor(Math.random()*hearts.length)];
        h.style.left = Math.random() * 100 + "vw";
        h.style.animationDuration = 4 + Math.random() * 3 + "s";
        h.style.fontSize = 16 + Math.random() * 20 + "px";
        document.body.appendChild(h);
        setTimeout(()=>h.remove(), 7000);
    }, 400);
</script>

</body>
</html>
