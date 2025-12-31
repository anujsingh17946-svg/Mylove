<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Happy New Year Love 💗</title>
<style>
    body {
        font-family: Arial, sans-serif;
        background: #ffe6f0;
        color: #c4006a;
        text-align: center;
        padding-top: 100px;
        overflow: hidden;
    }
    h1 {
        font-size: 40px;
    }
    #loveCounter {
        font-size: 50px;
        margin-top: 50px;
        color: #ff1493;
    }
    .sparkle {
        position: fixed;
        font-size: 20px;
        color: gold;
        animation: sparkleAnim 1.5s infinite;
    }
    @keyframes sparkleAnim {
        0% {transform: translateY(0) scale(1);}
        50% {transform: translateY(-20px) scale(1.5);}
        100% {transform: translateY(0) scale(1);}
    }
</style>
</head>
<body>

<h1>🎉 Happy New Year Muskan! 🎉</h1>
<p>Calculating how much I love you...</p>
<div id="loveCounter">0</div>

<div id="sparkles"></div>

<script>
// Love counter logic
let counter = 0;
let loveDisplay = document.getElementById('loveCounter');

function updateCounter() {
    counter += Math.floor(Math.random()*1000000);
    if(counter > 9999999999999){
        loveDisplay.innerHTML = '∞ 💗';
        clearInterval(counterInterval);
    } else {
        loveDisplay.innerHTML = counter.toLocaleString();
    }
}

let counterInterval = setInterval(updateCounter, 50);

// Sparkle animation
const sparklesContainer = document.getElementById('sparkles');
function createSparkle() {
    const s = document.createElement('div');
    s.className='sparkle';
    s.style.left = Math.random()*window.innerWidth+'px';
    s.style.top = Math.random()*window.innerHeight+'px';
    s.innerHTML = '✨';
    sparklesContainer.appendChild(s);
    setTimeout(()=>sparklesContainer.removeChild(s),1500);
}
setInterval(createSparkle,200);
</script>

</body>
</html><!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Aaj ka Din</title>
<style>
body {font-family: Arial,sans-serif; background:#ffe6f0; color:#4a004a; padding:40px; text-align:left; overflow-x:hidden;}
a{color:#c4006a; text-decoration:none; font-weight:bold;}
.rose{position:fixed; top:-50px; font-size:24px; color:red; z-index:0; pointer-events:none; animation-name:fall; animation-timing-function:linear; animation-iteration-count:infinite;}
@keyframes fall{0% {transform:translateY(-50px) rotate(0deg);} 100% {transform:translateY(100vh) rotate(360deg);}}
</style>
</head>
<body>

<h1>💗 Aaj ka Din 💗</h1>

<p>
Mere liye aaj ka din bohot accha tha..subah ki starting waise hi hui jaise pehle jab ham relationship me aye the tab hua karti thi...🫂💗  
Or aajka din bohot pyara tha idk tumhare liye kaisa tha but mere liye bohot pyara tha wo alag baat hai aaj me thoda busy tha or thoda tum to utni baat nahi hui but subah bohot acche se baat hui wo bohot pyari cheez thi or ykw mussu 🫂🫂💗
</p>

<p>
<a href="rose.html">➡ Next: My First Rose & Chocolate</a>
</p>

<div id="roses"></div>
<script>
const rosesContainer=document.getElementById('roses');
function createRose(){const r=document.createElement('div');r.className='rose';r.style.left=Math.random()*window.innerWidth+'px';r.style.animationDuration=(3+Math.random()*5)+'s';r.innerHTML='🌹';rosesContainer.appendChild(r);setTimeout(()=>rosesContainer.removeChild(r),8000);}
setInterval(createRose,500);
</script>

</body>
</html><!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>My First Rose</title>
<style>
body{font-family:Arial,sans-serif; background:#fff0f5; color:#4a004a; padding:40px; text-align:left; overflow-x:hidden;}
a{color:#c4006a; text-decoration:none; font-weight:bold;}
.rose{position:fixed; top:-50px; font-size:24px; color:red; z-index:0; pointer-events:none; animation-name:fall; animation-timing-function:linear; animation-iteration-count:infinite;}
@keyframes fall{0%{transform:translateY(-50px) rotate(0deg);}100%{transform:translateY(100vh) rotate(360deg);}}
</style>
</head>
<body>

<h1>🌹 My First Rose 🌹</h1>

<p>
aaj tum mere liye rose leke ayi..mujhe pehli bar kisi ne rose diya (isse pehle family cousin sister friend kisi ne nahi diya) 🫂💗 ye meri life ka first rose tha or mujhe nahi pata tha mai kaise react karu to me bas blush kare ja raha tha mujhe kuch nahi bolna tha me bas khush hona cahta tha 🫂🫂💗  
pata hai tum pure time padh rahi thi or agar piche mudke dekhti to wo pure 1 ghante me bas hase ja raha tha that rose was just very important for me 💗💗
</p>

<p>
Wo chocolate ke liye bhi bohot bohot thank you me usko kisi ke sath share nahi karne wala me wo akela khaunga maine socha tha tumhare sath share karunga but tumhara fast tha or tumhara apne hatho se kuch mere liye bana ke lana mere liye bohot special hai mussu...
</p>

<p>
<a href="promise.html">➡ Next: Promise & Future</a>
</p>

<div id="roses"></div>
<script>
const rosesContainer=document.getElementById('roses');
function createRose(){const r=document.createElement('div');r.className='rose';r.style.left=Math.random()*window.innerWidth+'px';r.style.animationDuration=(3+Math.random()*5)+'s';r.innerHTML='🌹';rosesContainer.appendChild(r);setTimeout(()=>rosesContainer.removeChild(r),8000);}
setInterval(createRose,500);
</script>

</body>
</html><!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Promise & Love</title>
<style>
body{font-family:Arial,sans-serif; background:#ffeaf4; color:#4a004a; padding:40px; text-align:left; overflow-x:hidden;}
a{color:#c4006a; text-decoration:none; font-weight:bold;}
.rose{position:fixed; top:-50px; font-size:24px; color:red; z-index:0; pointer-events:none; animation-name:fall; animation-timing-function:linear; animation-iteration-count:infinite;}
@keyframes fall{0%{transform:translateY(-50px) rotate(0deg);}100%{transform:translateY(100vh) rotate(360deg);}}
</style>
</head>
<body>

<h1>🫂 My Promise to You 🫂</h1>

<p>
tumhe me dil se pyar karta hu mussu..and i promise I am not gonna leave you for rest of my life...🫂🫂💗 me hamesha rahunga baccha...🫂💗 jab tak tum rakhogi tab tak rahunga i love you muskan 🫂🫂💗
</p>

<p>
tumhare ane ke baad aisa feel hone laga me bhi apne life ka main character hu otherwise hamesha bas sabke bare me sochta rehta tha tumhare ane ke baad pata chala ki me bhi special hu or deserve karta hu kisi ka pyar..🫂🫂💗 tumne mujhe jitna pyar diya itna mujhe kabhi kisi se nahi mila...✨🫂💗 thank you for everything baccha..2025 mere ek bohot pyara saal tha...
</p>

<p>
<a href="thankyou.html">➡ Next: Final Thank You</a>
</p>

<div id="roses"></div>
<script>
const rosesContainer=document.getElementById('roses');
function createRose(){const r=document.createElement('div');r.className='rose';r.style.left=Math.random()*window.innerWidth+'px';r.style.animationDuration=(3+Math.random()*5)+'s';r.innerHTML='🌹';rosesContainer.appendChild(r);setTimeout(()=>rosesContainer.removeChild(r),8000);}
setInterval(createRose,500);
</script>

</body>
</html><!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Thank You Muskan</title>
<style>
body{font-family:Arial,sans-serif; background:#ffe6f0; color:#4a004a; padding:40px; text-align:center; overflow:hidden;}
.rose{position:fixed; top:-50px; font-size:24px; color:red; z-index:0; pointer-events:none; animation-name:fall; animation-timing-function:linear; animation-iteration-count:infinite;}
@keyframes fall{0%{transform:translateY(-50px) rotate(0deg);}100%{transform:translateY(100vh) rotate(360deg);}}
.sparkle{position:fixed; font-size:20px; color:#ff1493; z-index:2; pointer-events:none; animation-name:sparkleAnim; animation-duration:1.5s; animation-iteration-count:infinite;}
@keyframes sparkleAnim{0%{transform:translateY(0) scale(1);}50%{transform:translateY(-20px) scale(1.5);}100%{transform:translateY(0) scale(1);}}
</style>
</head>
<body>

<h1>🫂💗 Thank you Muskan for choosing me 💗🫂</h1>
<p>🌟✨🌹✨🌟</p>

<audio autoplay loop>
  <source src="https://www.bensound.com/bensound-music/bensound-sweet.mp3" type="audio/mpeg">
</audio>

<div id="roses"></div>
<div id="sparkles"></div>

<script>
const rosesContainer=document.getElementById('roses');
function createRose(){const r=document.createElement('div');r.className='rose';r.style.left=Math.random()*window.innerWidth+'px';r.style.animationDuration=(3+Math.random()*5)+'s';r.innerHTML='🌹';rosesContainer.appendChild(r);setTimeout(()=>rosesContainer.removeChild(r),8000);}
setInterval(createRose,500);

const sparklesContainer=document.getElementById('sparkles');
function createSparkle(){const s=document.createElement('div');s.className='sparkle';s.style.left=Math.random()*window.innerWidth+'px';s.style.top=Math.random()*window.innerHeight+'px';s.innerHTML='✨';sparklesContainer.appendChild(s);setTimeout(()=>sparklesContainer.removeChild(s),1500);}
setInterval(createSparkle,200);
</script>

</body>
</html>
