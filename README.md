# birthday-wishes
<!DOCTYPE html>

<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Happy Birthday Aishwarya!</title>

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:'Poppins',sans-serif;
}

body{
    background: linear-gradient(135deg,#ff9ad5,#8ec5fc);
    color:white;
    text-align:center;
    overflow-x:hidden;
}

.hero{
    min-height:100vh;
    display:flex;
    flex-direction:column;
    justify-content:center;
    align-items:center;
    padding:20px;
}

h1{
    font-size:3rem;
    animation: glow 2s infinite alternate;
}

@keyframes glow{
    from{ text-shadow:0 0 10px #fff; }
    to{ text-shadow:0 0 30px #fff,0 0 50px #ff69b4; }
}

.message{
    max-width:700px;
    margin-top:20px;
    font-size:1.3rem;
    line-height:1.7;
}

.gallery{
    padding:50px 20px;
}

.gallery h2{
    margin-bottom:25px;
}

.photos{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(220px,1fr));
    gap:20px;
}

.photos img{
    width:100%;
    height:300px;
    object-fit:cover;
    border-radius:20px;
    box-shadow:0 8px 20px rgba(0,0,0,0.3);
}

button{
    margin:40px 0;
    padding:15px 35px;
    border:none;
    border-radius:50px;
    background:white;
    color:#ff4fa3;
    font-size:1rem;
    cursor:pointer;
    font-weight:bold;
}

#surprise{
    display:none;
    font-size:1.5rem;
    padding:20px;
}

.balloon{
    position:fixed;
    bottom:-150px;
    font-size:40px;
    animation: float 10s linear infinite;
}

@keyframes float{
    0%{
        transform:translateY(0);
    }
    100%{
        transform:translateY(-120vh);
    }
}
</style>

</head>

<body>

<div class="hero">
    <h1>🎂 Happy Birthday Aishwarya 🎂</h1>

```
<div class="message">
    Happy birthday to my favorite troublemaker! 💖<br><br>
    Life is never boring, and I'm never anything but happy when you're around.
    Thank you for all the laughter, memories, and crazy moments we share.
    May your day be filled with happiness, love, and everything you wish for.
    You deserve the very best today and always. 🎉✨
</div>
```

</div>

<section class="gallery">
    <h2>📸 Our Memories</h2>

```
<div class="photos">
    <img src="photo1.jpg" alt="">
    <img src="photo2.jpg" alt="">
    <img src="photo3.jpg" alt="">
    <img src="photo4.jpg" alt="">
</div>
```

</section>

<button onclick="showSurprise()">🎁 Click For A Surprise</button>

<div id="surprise">
    💙🌸 Dear Aishwarya 🌸💙<br><br>
    No matter how many birthdays come and go,
    you'll always be one of the most special people in my life.
    Thank you for being my best friend, my partner in crime,
    and the reason behind countless smiles.
    Happy Birthday! 🎂✨💖
</div>

<!-- Background Music -->

<audio autoplay loop>
    <source src="birthday-song.mp3" type="audio/mpeg">
</audio>

<script>
function showSurprise(){
    document.getElementById("surprise").style.display="block";
}

for(let i=0;i<25;i++){
    let balloon=document.createElement("div");
    balloon.className="balloon";
    balloon.innerHTML=Math.random()>0.5 ? "🎈" : "🎉";
    balloon.style.left=Math.random()*100+"vw";
    balloon.style.animationDuration=(6+Math.random()*8)+"s";
    document.body.appendChild(balloon);
}
</script>

</body>
</html>
