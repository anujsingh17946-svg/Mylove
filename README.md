<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Our Special Moments</title>
<style>
    body {
        font-family: Arial, sans-serif;
        background: #fff0f5;
        color: #4a004a;
        padding: 40px;
        text-align: center;
        overflow-x: hidden;
        transition: background 0.5s;
    }

    button {
        background-color: #c4006a;
        color: white;
        border: none;
        padding: 10px 20px;
        margin: 10px;
        cursor: pointer;
        border-radius: 5px;
        font-weight: bold;
        font-size: 16px;
    }

    button:hover {
        background-color: #a00055;
    }

    section {
        display: none;
        animation: fadeIn 0.5s;
        position: relative;
        z-index: 1;
    }

    section.active {
        display: block;
    }

    @keyframes fadeIn {
        from {opacity:0;}
        to {opacity:1;}
    }

    /* Dramatic "No" effect */
    .shake {
        animation: shake 0.5s;
    }
    @keyframes shake {
        0% { transform: translate(5px,0); }
        25% { transform: translate(-5px,0); }
        50% { transform: translate(5px,0); }
        75% { transform: translate(-5px,0); }
        100% { transform: translate(0,0); }
    }

    .hidden {
        display: none;
    }

    /* Rose falling animation */
    .rose {
        position: fixed;
        top: -50px;
        font-size: 24px;
        color: red;
        z-index: 0;
        pointer-events: none;
        animation-name: fall;
        animation-timing-function: linear;
        animation-iteration-count: infinite;
    }

    @keyframes fall {
        0% {transform: translateY(-50px) rotate(0deg);}
        100% {transform: translateY(100vh) rotate(360deg);}
    }

    /* Sparkle animation for final page */
    .sparkle {
        position: fixed;
        font-size: 20px;
        color: #ff1493;
        z-index: 2;
        pointer-events: none;
        animation-name: sparkleAnim;
        animation-duration: 1.5s;
        animation-iteration-count: infinite;
    }
    @keyframes sparkleAnim {
        0% {transform: translateY(0) scale(1);}
        50% {transform: translateY(-20px) scale(1.5);}
        100% {transform: translateY(0) scale(1);}
    }

</style>
</head>
<body>

<h1>🫂 Our Special Moments 🫂</h1>

<!-- Background Music -->
<audio autoplay loop>
    <source src="https://www.bensound.com/bensound-music/bensound-sweet.mp3" type="audio/mpeg">
</audio>

<!-- Rose falling elements -->
<div id="roses"></div>

<!-- Sparkle container -->
<div id="sparkles"></div>

<!-- First slide: Do you love me -->
<section id="loveCheck" class="active">
    <h2>💖 Do you love me? 💖</h2>
    <button onclick="chooseLove('yes')">Yes</button>
    <button onclick="chooseLove('no')">No</button>
    <p id="dramaticText" class="hidden">😢 Oh no! How could you not? 😢</p>
</section>

<!-- Main content -->
<section id="day">
    <h2>💗 Aaj ka Din 💗</h2>
    <p>
        Mere liye aaj ka din bohot accha tha. Subah ki starting bilkul waise hi hui
        jaise pehle jab hum relationship me aaye the.  
        Aaj ka din bohot pyara tha, chahe hum zyada baat nahi kar paaye,
        lekin subah ki baatein dil se bohot special thi 🫂
    </p>
    <p>
        Main thoda busy tha, tum bhi padh rahi thi,  
        lekin phir bhi wo connection, wo feeling… sab perfect tha 💗
    </p>
</section>

<section id="rose">
    <h2>🌹 My First Rose 🌹</h2>
    <p>
        Aaj tum mere liye rose leke aayi.  
        Ye meri life ka <strong>pehla rose</strong> tha.  
        Isse pehle kisi ne nahi diya… family, friends, koi bhi nahi.
    </p>
    <p>
        Mujhe nahi pata tha kaise react karun, bas blush hi karta raha 🫂💗  
        Agar tum piche mudke dekhti, to ek ghante tak bas hasta hi rehta.
    </p>
    <p>
        Wo rose meri zindagi ka bohot important hissa ban gaya.
        Main use hamesha sambhal ke rakhunga 💗
    </p>
    <p>
        Chocolate ke liye bhi thank you.  
        Main use kisi ke saath share nahi karunga, sirf apne liye 💗  
        Tumhare chote chote gestures hi mere liye sab kuch hain.
    </p>
</section>

<section id="promise">
    <h2>🫂 My Promise to You 🫂</h2>
    <p>
        Tumhare aane ke baad mujhe laga ki main bhi apni life ka main character hoon 💗  
        Tumne mujhe wo feeling di jo mujhe kabhi kisi se nahi mili.
    </p>
    <p>
        Main maanta hoon, maine is saal bohot galtiyan ki.
        Tumhe hurt kiya, pareshan kiya. Iske liye dil se sorry 💔
    </p>
    <p>
        2026 me main apne career pe bhi dhyaan dunga aur hamare relationship pe bhi.
        Koi sacrifice nahi hoga 🫂
    </p>
    <p>
        Main promise karta hoon ki:
        <ul>
            <li>Main tumhe samajhne ki koshish karunga</li>
            <li>Main tumhara saath kabhi nahi chhodunga</li>
            <li>Main hamesha tumhara rahunga</li>
        </ul>
    </p>
    <p>
        I love you Muskan 💗  
        Agale 1000 saal tak… jab tak Yamraj khud alag na kare 🧿
    </p>
</section>

<section id="thankyou">
    <h2>🫂💗 Thank you Muskan for choosing me 💗🫂</h2>
    <p>🌟✨🌹✨🌟</p>
</section>

<script>
// Generate falling roses
const rosesContainer = document.getElementById('roses');
function createRose() {
    const rose = document.createElement('div');
    rose.className = 'rose';
    rose.style.left = Math.random() * window.innerWidth + 'px';
    rose.style.animationDuration = (3 + Math.random() * 5) + 's';
    rose.innerHTML = '🌹';
    rosesContainer.appendChild(rose);
    setTimeout(() => rosesContainer.removeChild(rose), 8000);
}
setInterval(createRose, 500);

// Sparkle animation for final page
const sparklesContainer = document.getElementById('sparkles');
function createSparkle() {
    const sparkle = document.createElement('div');
    sparkle.className = 'sparkle';
    sparkle.style.left = Math.random() * window.innerWidth + 'px';
    sparkle.style.top = Math.random() * window.innerHeight + 'px';
    sparkle.innerHTML = '✨';
    sparklesContainer.appendChild(sparkle);
    setTimeout(() => sparklesContainer.removeChild(sparkle), 1500);
}

// Create continuous sparkles on final page
setInterval(() => {
    if(document.getElementById('thankyou').classList.contains('active')) {
        createSparkle();
    }
}, 200);

// Love choice logic
function chooseLove(choice) {
    if(choice === 'yes') {
        document.getElementById('loveCheck').classList.remove('active');
        document.getElementById('day').classList.add('active');
        document.getElementById('rose').classList.add('active');
        document.getElementById('promise').classList.add('active');
        // Show final thank you page after 2 seconds
        setTimeout(() => {
            document.getElementById('thankyou').classList.add('active');
        }, 2000);
    } else {
        const loveCheck = document.getElementById('loveCheck');
        const text = document.getElementById('dramaticText');
        loveCheck.classList.add('shake');
        text.classList.remove('hidden');
        setTimeout(() => loveCheck.classList.remove('shake'), 500);
    }
}
</script>

</body>
</html>
