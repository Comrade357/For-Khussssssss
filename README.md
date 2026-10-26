# For-Khussssssss

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#1b102b">
<title>For Khusssss ♡</title>

<style>
@import url('https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;600;700&family=Playfair+Display:wght@500;600;700&display=swap');

:root{
  --pink:#ffb7df;
  --pink2:#ff75c8;
  --purple:#bba3ff;
  --purple2:#8059e8;
  --bg:#160f25;
  --panel:#261a3b;
  --white:#fff5ff;
  --muted:#d3c5e9;
  --gold:#ffe3a7;
}

*{box-sizing:border-box;scroll-behavior:smooth}
body{
  margin:0;
  font-family:'DM Sans',sans-serif;
  background:
    radial-gradient(ellipse at 15% 5%,#512d6b66,transparent 40%),
    radial-gradient(ellipse at 85% 30%,#6e337366,transparent 40%),
    var(--bg);
  color:var(--white);
  overflow-x:hidden;
}
button,input,textarea,select{font:inherit}
button{cursor:pointer}
a{color:inherit;text-decoration:none}
.hidden{display:none!important}

#magic{
  position:fixed;
  inset:0;
  overflow:hidden;
  pointer-events:none;
  z-index:10;
}
.floating{
  position:absolute;
  bottom:-50px;
  opacity:0;
  animation:floatUp linear forwards;
  text-shadow:0 0 12px #ffb7df;
}
@keyframes floatUp{
  0%{transform:translateY(0) rotate(0);opacity:0}
  10%{opacity:.8}
  90%{opacity:.65}
  100%{transform:translateY(-115vh) rotate(360deg);opacity:0}
}
.burst{
  position:fixed;
  z-index:100;
  pointer-events:none;
  animation:burst .9s ease-out forwards;
}
@keyframes burst{
  to{transform:translate(var(--x),var(--y)) scale(.1) rotate(180deg);opacity:0}
}

.topbar{
  position:sticky;top:0;z-index:20;
  display:flex;align-items:center;justify-content:space-between;
  gap:12px;padding:14px 5%;
  background:#160f25d9;backdrop-filter:blur(18px);
  border-bottom:1px solid #ffffff13;
}
.brand{font-weight:700;color:var(--pink);letter-spacing:.5px}
nav{display:flex;gap:18px;font-size:13px;color:var(--muted)}
nav a:hover{color:var(--pink)}
.small-btn{
  border:1px solid #ffffff2c;background:#ffffff0c;
  color:white;padding:8px 12px;border-radius:30px;font-size:12px
}

section{padding:85px 6%;position:relative}
.hero{
  min-height:90vh;display:flex;flex-direction:column;
  justify-content:center;align-items:center;text-align:center;
  overflow:hidden;
}
.orb{
  position:absolute;width:300px;height:300px;border-radius:50%;
  filter:blur(75px);opacity:.22;pointer-events:none
}
.orb.one{background:#ff75c8;top:10%;left:-100px}
.orb.two{background:#8661ff;bottom:0;right:-100px}
.eyebrow{
  color:var(--pink);text-transform:uppercase;
  letter-spacing:3px;font-size:11px;font-weight:700
}
h1,h2,h3{font-family:'Playfair Display',serif}
h1{font-size:clamp(48px,10vw,100px);line-height:1.06;margin:20px 0}
h1 span,h2 em{font-style:normal;color:var(--pink)}
h1 .heart{color:var(--purple)}
h2{font-size:clamp(32px,5vw,54px);margin:12px 0 25px}
h3{font-size:24px;margin-top:0}
.lead,.copy{max-width:680px;line-height:1.9;color:var(--muted)}
.primary,.secondary{
  border:0;border-radius:40px;padding:14px 23px;
  transition:.25s;display:inline-flex;align-items:center;gap:10px;
}
.primary{
  color:#28152f;font-weight:700;
  background:linear-gradient(120deg,var(--pink),var(--purple));
  box-shadow:0 0 30px #d58bff2b;
}
.secondary{
  background:#ffffff0c;color:var(--white);
  border:1px solid #ffffff25;
}
.primary:hover,.secondary:hover{transform:translateY(-3px);filter:brightness(1.1)}
.panel{
  background:linear-gradient(145deg,#ffffff0d,#ffffff04);
  border:1px solid #ffffff1b;border-radius:24px;
  padding:25px;backdrop-filter:blur(12px);
  box-shadow:0 15px 50px #00000012;
}
.countdown{margin:30px 0;min-width:min(90%,460px)}
#timer{font-size:clamp(18px,4vw,30px);color:var(--gold)}
#timer b{color:white}
#birthday-note{font-size:12px;color:var(--muted)}
.scroll{margin-top:65px;color:#a99abf;font-size:11px;letter-spacing:2px}
.center{text-align:center}
.grid{display:grid;gap:18px}
.gallery{grid-template-columns:repeat(auto-fit,minmax(145px,1fr))}
.gallery img{
  width:100%;height:210px;object-fit:cover;border-radius:17px;
  border:1px solid #ffffff24;transition:.3s;cursor:pointer;
}
.gallery img:hover{transform:translateY(-5px) rotate(-1deg);box-shadow:0 10px 35px #ff8cce35}
.timeline{margin-top:35px}
.timeline-item{padding:15px;border-left:2px solid var(--purple);margin:10px 0}
.timeline-item span{color:var(--pink);font-weight:700}
.two{grid-template-columns:repeat(auto-fit,minmax(260px,1fr))}
.gift-grid{grid-template-columns:repeat(auto-fit,minmax(130px,1fr))}
.gift{
  padding:24px 12px;text-align:center;border-radius:18px;
  background:#ffffff09;border:1px solid #ffffff19;color:white;
  transition:.25s;min-height:140px
}
.gift:hover{transform:translateY(-5px);border-color:var(--pink)}
.gift .emoji{font-size:36px;display:block;margin-bottom:10px}
.gift p{font-size:12px;color:var(--muted)}
.reason-grid{grid-template-columns:repeat(auto-fit,minmax(145px,1fr))}
.reason{
  min-height:115px;border:1px solid #ffffff1b;border-radius:16px;
  background:#ffffff08;color:white;padding:18px;
}
.reason.open{background:#a77be72b;border-color:var(--pink)}
.reason small{display:block;color:var(--pink);margin-bottom:10px}
input,textarea,select{
  background:#ffffff0b;color:white;border:1px solid #ffffff2a;
  border-radius:12px;padding:12px;width:100%;margin:6px 0;
}
option{background:#261a3b}
textarea{min-height:100px;resize:vertical}
.inline{display:flex;gap:8px;align-items:center}
.inline button{flex-shrink:0}
.status{color:var(--pink);line-height:1.7}
.envelope{
  display:block;margin:25px auto;padding:30px 50px;
  border-radius:20px;background:linear-gradient(135deg,#ffb7df,#bba3ff);
  color:#28152f;border:0;font-size:18px
}
.envelope span{display:block;font-size:55px}
.letter{max-width:750px;margin:25px auto;line-height:1.9;color:var(--muted)}
.signature{color:var(--pink);font-family:'Playfair Display',serif;font-size:23px}
.cake{text-align:center}
.cake-art{font-size:75px;margin:20px}
.flame{color:var(--gold);animation:twinkle 1s infinite alternate}
@keyframes twinkle{to{opacity:.45;transform:scale(.8)}}
.jar{font-size:75px;color:var(--pink);text-shadow:0 0 30px #ff8cce;margin:15px}
.flower-row{display:flex;justify-content:center;gap:15px;flex-wrap:wrap}
.flower{font-size:40px;background:none;border:0;color:var(--pink)}
.hug-heart{font-size:65px;background:none;border:0;color:var(--pink);animation:heartbeat 1.3s infinite}
@keyframes heartbeat{50%{transform:scale(1.15)}}
#constellation{display:flex;justify-content:center;gap:20px;flex-wrap:wrap;font-size:35px}
#constellation button{background:none;border:0;color:var(--gold)}
#video{width:100%;max-width:650px;border-radius:18px}
.final-photo img{width:min(85%,380px);max-height:450px;object-fit:cover;border-radius:24px;border:2px solid #ffb7df}
.final-message{padding:30px;background:#ffffff0a;border-radius:24px;margin-top:25px}
footer{text-align:center;padding:35px;color:#a99abf;font-size:12px}
@media(max-width:650px){
 nav{display:none}
 .topbar{padding:12px 4%}
 section{padding:65px 5%}
 .panel{padding:19px}
 .inline{flex-wrap:wrap}
 .inline button{width:100%;justify-content:center}
 .gallery img{height:170px}
}
</style>
</head>

<body>
<div id="magic"></div>

<header class="topbar">
  <a class="brand" href="#home">✦ For Khusssss</a>
  <nav>
    <a href="#memories">Memories</a>
    <a href="#surprises">Surprises</a>
    <a href="#wishes">Wishes</a>
  </nav>
  <button class="small-btn" id="magicToggle">✨ Magic ON</button>
  <button class="small-btn" id="musicToggle">♫ Music</button>
</header>

<audio id="music" src="Song22.mp3" loop preload="metadata"></audio>

<main>
<!-- 1-6: WELCOME EXPERIENCE -->
<section class="hero" id="home">
 <div class="orb one"></div><div class="orb two"></div>
 <p class="eyebrow">A little universe made just for you</p>
 <h1>Happy Birthday,<br><span>Khusssss</span> <span class="heart">♡</span></h1>
 <p class="lead">For my sister, my forever friend, and one of the brightest stars in my sky.</p>
 <div class="panel countdown">
  <p class="eyebrow">Counting down to your special day</p>
  <div id="timer">Loading birthday magic...</div>
  <p id="birthday-note">November 5, 2026</p>
 </div>
 <button class="primary" onclick="enterMagic()">Enter your birthday universe ✦</button>
 <div class="scroll">SCROLL TO EXPLORE ↓</div>
</section>

<section class="center">
 <p class="eyebrow">A birthday note</p>
 <h2>Today, the universe celebrates <em>you.</em></h2>
 <p class="copy" style="margin:auto">You make ordinary days warmer, memories brighter, and our family more special. This little website is a collection of love, laughter, and all the things I hope you never forget.</p>
</section>

<!-- 7-10: MEMORIES -->
<section id="memories">
 <p class="eyebrow">Chapter one · our story</p>
 <h2>Little moments, <em>forever memories.</em></h2>
 <p class="copy">Your photos are waiting here. Tap any picture to see it bigger.</p>
 <div class="grid gallery" id="gallery"></div>

 <div class="panel timeline">
  <h3>Our sibling timeline</h3>
  <div class="timeline-item"><span>✦ Then</span><p>All the little beginnings that became our story.</p></div>
  <div class="timeline-item"><span>♡ Along the way</span><p>The jokes, adventures, and moments only we understand.</p></div>
  <div class="timeline-item"><span>∞ Always</span><p>No matter where life takes us, I’ll always be cheering for you.</p></div>
 </div>

 <div class="panel" style="margin-top:20px">
  <h3>Our memory scrapbook</h3>
  <textarea id="memoryNote" placeholder="Write a favorite memory here..."></textarea>
  <button class="secondary" onclick="saveMemory()">Save memory note</button>
  <p id="memorySaved" class="status"></p>
 </div>

 <div class="panel" style="margin-top:20px">
  <h3>🎬 A little memory movie</h3>
  <p class="copy">A video memory from your collection.</p>
  <video id="video" controls playsinline>
   <source src="K11.mp4" type="video/mp4">
   Your browser does not support this video.
  </video>
 </div>
</section>

<!-- 11-15: LETTER AND LOVE -->
<section id="letter" class="center">
 <p class="eyebrow">Chapter two · from my heart</p>
 <h2>A letter, <em>just for you.</em></h2>
 <button class="envelope" id="openLetter" onclick="openLetter()">
  <span>✉</span>Tap to open your letter
 </button>
 <article class="panel letter hidden" id="letterContent">
  <h3>Dear Khusssss,</h3>
  <p>Happy birthday to the sweetest sister. I hope your days are filled with courage, peace, laughter, and people who love you exactly as you are.</p>
  <p>Keep dreaming big and being your wonderful self. Whatever happens, remember you will always have me in your corner.</p>
  <p>May this year bring you beautiful surprises and a thousand reasons to smile.</p>
  <p class="signature">With all my love, always ♡</p>
 </article>
 <div class="panel" style="margin-top:25px">
  <h3>A message from the future</h3>
  <p class="copy">Dear future Khusssss: I hope you’re proud of how far you’ve come. Keep choosing joy, keep trusting your heart, and never stop believing that wonderful things are possible.</p>
 </div>
</section>

<!-- 16-24: SURPRISES -->
<section id="surprises">
 <p class="eyebrow">Chapter three · tiny wonders</p>
 <h2>Surprises made of <em>stardust.</em></h2>
 <p class="copy">Open every gift. Collect stars. Find your ultimate surprise.</p>
 <div class="grid gift-grid" id="gifts"></div>

 <div class="panel" style="margin-top:25px">
  <h3>🔐 The secret treasure chest</h3>
  <p>Enter the birthday day number to open the chest.</p>
  <div class="inline"><input id="treasureCode" placeholder="Birthday code" inputmode="numeric"><button class="secondary" onclick="unlockChest()">Unlock</button></div>
  <p class="status" id="treasureResult"></p>
 </div>

 <div class="panel center" style="margin-top:20px">
  <h3>🌌 A hidden room</h3>
  <p>Find the tiny star below. Tap it five times.</p>
  <button class="secondary" id="secretStar" onclick="findSecret()">✦</button>
  <p class="status hidden" id="hiddenRoom">You found the secret room! You are loved more than all the stars in this universe. ♡</p>
 </div>

 <div class="panel center" style="margin-top:20px">
  <h3>✨ The magic button</h3>
  <p>Tap for a little burst of birthday magic.</p>
  <button class="primary" onclick="burst(event)">Make magic ✨</button>
 </div>
</section>

<!-- 25-30: FUN -->
<section id="play">
 <p class="eyebrow">Chapter four · play time</p>
 <h2>Let’s make a little <em>magic.</em></h2>

 <div class="grid two">
  <div class="panel center">
   <h3>🎂 Make a birthday wish</h3>
   <div class="cake-art"><div class="flame" id="flame">✦</div>🕯️🎂</div>
   <p id="cakeMessage">Make a wish, then blow out the candle.</p>
   <button class="primary" id="blow" onclick="blowCandle()">Blow out candle</button>
   <button class="secondary hidden" id="relight" onclick="relight()">Light it again</button>
  </div>

  <div class="panel center">
   <h3>💫 Sister quiz</h3>
   <p id="quizQuestion">Which is the best part of being siblings?</p>
   <div id="quizOptions"></div>
   <p class="status" id="quizResult"></p>
   <button class="secondary" onclick="nextQuiz()">Next question</button>
  </div>

  <div class="panel center">
   <h3>🖼 Guess the memory</h3>
   <p>Choose a memory and reveal a little clue.</p>
   <div class="inline">
    <select id="memoryChoice"><option>Memory 1</option><option>Memory 2</option><option>Memory 3</option><option>Memory 4</option></select>
    <button class="secondary" onclick="memoryClue()">Reveal clue</button>
   </div>
   <p class="status" id="clue"></p>
  </div>

  <div class="panel center">
   <h3>🗺 Birthday adventure</h3>
   <p id="adventureText">Choose a path to begin your tiny adventure.</p>
   <button class="secondary" onclick="adventure('garden')">Garden</button>
   <button class="secondary" onclick="adventure('moon')">Moon</button>
   <button class="secondary" onclick="adventure('castle')">Castle</button>
  </div>
 </div>
</section>

<!-- 31-38: WISHES AND MAGIC -->
<section id="wishes">
 <p class="eyebrow">Chapter five · wishes and wonders</p>
 <h2>May your wishes <em>find their way.</em></h2>

 <div class="grid two">
  <div class="panel center">
   <h3>🏺 The birthday wish jar</h3>
   <div class="jar">♡</div>
   <p id="jarWish">Tap to draw a wish from the jar.</p>
   <button class="primary" onclick="drawWish()">Draw a wish</button>
  </div>

  <div class="panel center">
   <h3>🌷 The birthday garden</h3>
   <div class="flower-row">
    <button class="flower" onclick="flowerWish(0)">✿</button>
    <button class="flower" onclick="flowerWish(1)">✾</button>
    <button class="flower" onclick="flowerWish(2)">❀</button>
    <button class="flower" onclick="flowerWish(3)">✽</button>
   </div>
   <p id="flowerMessage">Tap a flower to make it bloom.</p>
  </div>
 </div>

 <div class="panel" style="margin-top:20px">
  <h3>💌 Your birthday wish wall</h3>
  <p>Write a wish for yourself. It will float into the birthday sky.</p>
  <div class="inline"><input id="wishInput" placeholder="My wish for this year is..."><button class="secondary" onclick="postWish()">Send wish</button></div>
  <div id="wishCloud"></div>
 </div>

 <div class="panel center" style="margin-top:20px">
  <h3>☔ Compliment rain</h3>
  <p id="complimentText">You are thoughtful, strong, and wonderfully you.</p>
  <button class="secondary" onclick="complimentRain()">Let it rain compliments</button>
 </div>

 <div class="panel center" style="margin-top:20px">
  <h3>🫂 A virtual hug</h3>
  <button class="hug-heart" onclick="virtualHug()">♡</button>
  <p id="hugMessage">Tap the heart whenever you need a hug.</p>
 </div>
</section>

<!-- 39-43: 50 REASONS AND STARS -->
<section id="reasons">
 <p class="eyebrow">Chapter six · all the little reasons</p>
 <h2>50 reasons you’re <em>special.</em></h2>
 <p class="copy">Tap the cards to reveal the reasons. Each opened card earns a star.</p>
 <div class="grid reason-grid" id="reasonsGrid"></div>

 <div class="panel center" style="margin-top:30px">
  <h3>✨ Our sibling constellation</h3>
  <p>Tap a star to read a tiny promise.</p>
  <div id="constellation"></div>
  <p id="constellationMessage" class="status"></p>
 </div>
</section>

<!-- 44-50: GRAND FINALE AND FEATURES -->
<section class="center" id="finale">
 <p class="eyebrow">The last little chapter</p>
 <h2>One more thing, <em>my sister.</em></h2>
 <div class="final-photo"><img src="K12.jpg" alt="A special memory of Khusssss" onerror="this.src='K1.jpg'"></div>
 <p class="copy" style="margin:25px auto">No website could ever hold all the love and gratitude I have for you. I hope this birthday brings you a lifetime of reasons to shine.</p>
 <button class="primary" onclick="finale()">Make the universe sparkle ✨</button>
 <div class="final-message hidden" id="finalMessage">
  <h2>Happy Birthday, Khusssss! ♡</h2>
  <p>You are loved—today, tomorrow, and always.</p>
  <button class="secondary" onclick="replay()">Replay birthday magic</button>
 </div>
</section>
</main>

<footer>Made with love for Khusssss · November 5, 2026 ♡</footer>

<div id="lightbox" class="hidden" style="position:fixed;inset:0;background:#090611ed;z-index:90;display:grid;place-items:center;padding:20px" onclick="this.classList.add('hidden')">
 <img id="lightboxImage" style="max-width:95%;max-height:90vh;border-radius:20px" alt="Expanded memory">
</div>

<script>
/* FLOATING HEARTS AND SPARKLES */
let magicOn=true;
const magicLayer=document.getElementById('magic');
const symbols=['♡','♥','✦','✧','✨','⋆','💗'];
function floatMagic(){
 if(!magicOn)return;
 const el=document.createElement('span');
 el.className='floating';
 el.textContent=symbols[Math.floor(Math.random()*symbols.length)];
 el.style.left=Math.random()*100+'%';
 el.style.fontSize=(12+Math.random()*22)+'px';
 el.style.animationDuration=(7+Math.random()*9)+'s';
 magicLayer.appendChild(el);
 setTimeout(()=>el.remove(),17000);
}
setInterval(floatMagic,350);
document.getElementById('magicToggle').onclick=()=>{
 magicOn=!magicOn;
 document.getElementById('magicToggle').textContent=magicOn?'✨ Magic ON':'✨ Magic OFF';
 if(!magicOn)magicLayer.innerHTML='';
};

/* BIRTHDAY COUNTDOWN */
function updateTimer(){
 const target=new Date('2026-11-05T00:00:00').getTime();
 const now=Date.now();
 let diff=target-now;
 const el=document.getElementById('timer');
 if(diff<=0){
  el.innerHTML='🎉 It’s your birthday! 🎉';
  document.getElementById('birthday-note').textContent='Today is all about you, Khusssss!';
  return;
 }
 const days=Math.floor(diff/86400000);diff%=86400000;
 const hours=Math.floor(diff/3600000);diff%=3600000;
 const mins=Math.floor(diff/60000);diff%=60000;
 const secs=Math.floor(diff/1000);
 el.innerHTML=`<b>${days}</b> days <b>${hours}</b> hrs <b>${mins}</b> min <b>${secs}</b> sec`;
}
setInterval(updateTimer,1000);updateTimer();

/* MUSIC — browsers require a user gesture */
const music=document.getElementById('music');
document.getElementById('musicToggle').onclick=async()=>{
 try{
  if(music.paused){await music.play();document.getElementById('musicToggle').textContent='♫ Pause';}
  else{music.pause();document.getElementById('musicToggle').textContent='♫ Music';}
 }catch(e){alert('Please check that Song22.mp3 is uploaded in your repository.');}
};
function enterMagic(){
 document.getElementById('memories').scrollIntoView({behavior:'smooth'});
 music.play().catch(()=>{});
 document.getElementById('musicToggle').textContent='♫ Pause';
 burst();
}

/* PHOTO GALLERY */
const gallery=document.getElementById('gallery');
for(let i=1;i<=10;i++){
 const img=document.createElement('img');
 img.src=`K${i}.jpg`;
 img.alt=`Birthday memory ${i}`;
 img.loading='lazy';
 img.onerror=()=>{img.style.display='none'};
 img.onclick=()=>{
  document.getElementById('lightboxImage').src=img.src;
  document.getElementById('lightbox').classList.remove('hidden');
 };
 gallery.appendChild(img);
}

/* MEMORY NOTE */
function saveMemory(){
 const val=document.getElementById('memoryNote').value.trim();
 document.getElementById('memorySaved').textContent=val?'Your memory note is written here with love ♡':'Write a memory first.';
}

/* LETTER */
function openLetter(){
 document.getElementById('letterContent').classList.toggle('hidden');
 const btn=document.getElementById('openLetter');
 btn.innerHTML='<span>💌</span>Letter opened';
 burst();
}

/* SEVEN GIFTS */
const giftMessages=[
 'A wish: may your dreams come true.',
 'A memory: every laugh we shared.',
 'A compliment: your heart is beautiful.',
 'A promise: I will always support you.',
 'A photo: one little moment to treasure.',
 'A reminder: you are more than enough.',
 'The ultimate gift: a lifetime of sibling love.'
];
const gifts=document.getElementById('gifts');
giftMessages.forEach((msg,i)=>{
 const b=document.createElement('button');
 b.className='gift';
 b.innerHTML=`<span class="emoji">🎁</span><b>Secret Gift ${i+1}</b><p>Tap to open</p>`;
 b.onclick=()=>{
  b.innerHTML=`<span class="emoji">💖</span><b>Gift ${i+1}</b><p>${msg}</p>`;
  b.style.background='#bd8dfb24';
  b.dataset.open='yes';
  collectStar();
  burst();
 };
 gifts.appendChild(b);
});

/* TREASURE CHEST */
function unlockChest(){
 const code=document.getElementById('treasureCode').value.trim();
 const out=document.getElementById('treasureResult');
 if(code==='5'){
  out.textContent='🔓 Chest unlocked! Your treasure is this reminder: you are loved endlessly.';
  collectStar();burst();
 }else out.textContent='Not quite! Hint: your birthday is on the 5th.';
}

/* HIDDEN ROOM */
let secretCount=0;
function findSecret(){
 secretCount++;
 if(secretCount>=5){
  document.getElementById('hiddenRoom').classList.remove('hidden');
  collectStar();burst();
 }
}

/* CLICK MAGIC BURST */
function burst(event){
 const x=event?.clientX??window.innerWidth/2;
 const y=event?.clientY??window.innerHeight/2;
 for(let i=0;i<18;i++){
  const el=document.createElement('span');
  el.className='burst';
  el.textContent=symbols[Math.floor(Math.random()*symbols.length)];
  el.style.left=x+'px';el.style.top=y+'px';
  el.style.setProperty('--x',(Math.random()*220-110)+'px');
  el.style.setProperty('--y',(Math.random()*220-110)+'px');
  document.body.appendChild(el);setTimeout(()=>el.remove(),1000);
 }
}

/* CANDLE */
function blowCandle(){
 document.getElementById('flame').textContent='♡';
 document.getElementById('cakeMessage').textContent='Wish made! May it come true. ✨';
 document.getElementById('blow').classList.add('hidden');
 document.getElementById('relight').classList.remove('hidden');
 burst();
}
function relight(){
 document.getElementById('flame').textContent='✦';
 document.getElementById('cakeMessage').textContent='Make a wish, then blow out the candle.';
 document.getElementById('blow').classList.remove('hidden');
 document.getElementById('relight').classList.add('hidden');
}

/* QUIZ */
const quiz=[
 {q:'Which is the best part of being siblings?',a:['Having someone to share memories with','Never talking','Being strangers'],correct:0},
 {q:'What do I wish for you?',a:['A beautiful life','No happiness','No dreams'],correct:0},
 {q:'What will I always be?',a:['Your sibling and supporter','A stranger','A forgotten memory'],correct:0}
];
let quizIndex=0;
function renderQuiz(){
 const q=quiz[quizIndex];
 document.getElementById('quizQuestion').textContent=q.q;
 document.getElementById('quizResult').textContent='';
 const box=document.getElementById('quizOptions');box.innerHTML='';
 q.a.forEach((a,i)=>{
  const b=document.createElement('button');b.className='secondary';b.style.margin='5px';b.textContent=a;
  b.onclick=()=>{document.getElementById('quizResult').textContent=i===q.correct?'Correct! You know our bond. ♡':'Try again, birthday girl!';
   if(i===q.correct)collectStar();};
  box.appendChild(b);
 });
}
function nextQuiz(){quizIndex=(quizIndex+1)%quiz.length;renderQuiz()}
renderQuiz();

/* MEMORY CLUE */
function memoryClue(){
 const n=document.getElementById('memoryChoice').selectedIndex+1;
 document.getElementById('clue').textContent=`Memory ${n}: A little snapshot that keeps a moment alive. What do you remember about it?`;
}

/* ADVENTURE */
function adventure(path){
 const text={
  garden:'You entered the garden. A flower blooms just for you. May joy grow around you!',
  moon:'You reached the moon. Make a wish and send it among the stars.',
  castle:'You found the castle. You are the princess of this birthday universe!'
 };
 document.getElementById('adventureText').textContent=text[path];
 collectStar();burst();
}

/* WISH JAR */
const wishes=[
 'May your dreams become beautiful realities.',
 'May you always find reasons to smile.',
 'May you be surrounded by genuine love.',
 'May courage meet you whenever you need it.',
 'May your future be brighter than the stars.',
 'May every new chapter bring you joy.'
];
function drawWish(){
 document.getElementById('jarWish').textContent=wishes[Math.floor(Math.random()*wishes.length)];
 collectStar();burst();
}

/* FLOWER GARDEN */
const flowerWishes=[
 'May your happiness bloom every day.',
 'May your dreams grow tall and strong.',
 'May love surround you wherever you go.',
 'May every season bring you something beautiful.'
];
function flowerWish(i){
 document.getElementById('flowerMessage').textContent=flowerWishes[i];
 burst();
}

/* WISH WALL */
function postWish(){
 const input=document.getElementById('wishInput');
 const val=input.value.trim();
 if(!val)return;
 const p=document.createElement('p');
 p.textContent='✨ '+val+' ♡';
 p.style.color='#ffb7df';
 p.style.padding='10px';
 p.style.animation='floatUp 8s linear';
 document.getElementById('wishCloud').appendChild(p);
 input.value='';collectStar();burst();
}

/* COMPLIMENTS */
const compliments=[
 'You are thoughtful, strong, and wonderfully you.',
 'Your smile makes the world feel warmer.',
 'You deserve every beautiful thing life has to offer.',
 'Your kindness is a kind of magic.',
 'You are more loved than you know.',
 'Never forget how special you are.'
];
function complimentRain(){
 document.getElementById('complimentText').textContent=compliments[Math.floor(Math.random()*compliments.length)];
 burst();
}

/* VIRTUAL HUG */
function virtualHug(){
 document.getElementById('hugMessage').textContent='Sending you the biggest, warmest sibling hug. ♡';
 burst();
}

/* 50 REASONS */
const reasons=[
'Your beautiful smile','Your kind heart','Your courage','Your laughter','Your honesty',
'Your creativity','Your patience','Your strength','Your dreams','Your warm hugs',
'Your thoughtful words','Your caring nature','Your funny moments','Your lovely energy','Your uniqueness',
'Your determination','Your generosity','Your gentle soul','Your bright ideas','Your resilience',
'Your wonderful personality','Your little quirks','Your ability to care','Your hopeful heart','Your curiosity',
'Your confidence','Your compassion','Your loyalty','Your magic','Your beautiful spirit',
'Your love for family','Your sense of humor','Your willingness to grow','Your bright future','Your inner strength',
'Your amazing presence','Your sweet memories','Your kindness to others','Your individuality','Your joy',
'Your dreams for tomorrow','Your heart of gold','Your ability to inspire','Your beautiful laugh','Your sincerity',
'Your love','Your courage to try','Your endless potential','Your special place in my life','Simply being you'
];
let stars=0;
const reasonsGrid=document.getElementById('reasonsGrid');
reasons.forEach((reason,i)=>{
 const b=document.createElement('button');
 b.className='reason';
 b.innerHTML=`<small>Reason ${i+1} ✦</small><span>Tap to reveal</span>`;
 b.onclick=()=>{
  if(!b.classList.contains('open'))collectStar();
  b.classList.add('open');
  b.innerHTML=`<small>Reason ${i+1} ♡</small><span>${reason}</span>`;
  burst();
 };
 reasonsGrid.appendChild(b);
});

/* STARS AND CONSTELLATION */
function collectStar(){
 stars++;
 document.getElementById('constellationMessage').textContent=`You have collected ${stars} birthday stars! ✨`;
}
const constellation=document.getElementById('constellation');
for(let i=0;i<7;i++){
 const b=document.createElement('button');b.textContent='✦';
 b.onclick=()=>{
  const messages=[
   'I promise to cheer for your dreams.',
   'I promise to listen when you need me.',
   'I promise to celebrate your wins.',
   'I promise to remind you of your worth.',
   'I promise to be there through hard days.',
   'I promise to treasure our memories.',
   'I promise that you will always have family love.'
  ];
  document.getElementById('constellationMessage').textContent=messages[i];
  collectStar();burst();
 };
 constellation.appendChild(b);
}

/* GRAND FINALE */
function finale(){
 document.getElementById('finalMessage').classList.remove('hidden');
 for(let i=0;i<5;i++)setTimeout(()=>burst(),i*250);
 collectStar();
}
function replay(){window.scrollTo({top:0,behavior:'smooth'});}

/* OTHER FEATURE: CELEBRATION ON BIRTHDAY */
if(new Date().toISOString().slice(0,10)==='2026-11-05'){
 document.getElementById('birthday-note').textContent='Happy Birthday, Khusssss! 🎉';
}

/* REVEAL SECTION EFFECT */
const observer=new IntersectionObserver(entries=>{
 entries.forEach(e=>{
  if(e.isIntersecting){
   e.target.style.opacity=1;
   e.target.style.transform='translateY(0)';
  }
 });
},{threshold:.08});
document.querySelectorAll('section').forEach(s=>{
 s.style.opacity=0;s.style.transform='translateY(20px)';
 s.style.transition='opacity .8s ease,transform .8s ease';
 observer.observe(s);
});
document.querySelector('.hero').style.opacity=1;
document.querySelector('.hero').style.transform='none';
</script>
</body>
</html>
