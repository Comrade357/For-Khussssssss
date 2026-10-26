
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#10091e">
<title>For Khusssss ♡</title>

<style>
*{box-sizing:border-box}
html{scroll-behavior:smooth}
body{margin:0;background:#10091e;color:#fff0fb;font-family:Georgia,serif}
button,input{font:inherit}
button{cursor:pointer}
.hidden{display:none!important}

:root{
 --pink:#ffaddf;
 --purple:#bca0ff;
 --gold:#ffe7bd;
 --glass:rgba(255,255,255,.07);
}

body:before{
 content:"";position:fixed;inset:0;z-index:-1;
 background:radial-gradient(ellipse at 10% 10%,#70245e66,transparent 45%),
 radial-gradient(ellipse at 90% 75%,#44308177,transparent 45%),#10091e
}

/* FLOATING HEARTS AND SPARKLES */
.particle{
 position:absolute;bottom:-60px;pointer-events:none;
 animation:floatUp linear forwards;
 text-shadow:0 0 12px #ff8bd4,0 0 25px #ac83ff;
}
@keyframes floatUp{
 0%{transform:translateY(0) rotate(0);opacity:0}
 12%{opacity:.85}
 85%{opacity:.7}
 100%{transform:translateY(-115vh) rotate(330deg);opacity:0}
}
#lockMagic,#siteMagic{
 position:fixed;inset:0;overflow:hidden;pointer-events:none;z-index:1
}

/* LOCK SCREEN */
#birthdayLock{
 position:fixed;inset:0;z-index:9999;
 display:flex;align-items:center;justify-content:center;
 padding:16px;overflow:hidden;isolation:isolate;
 background:
 radial-gradient(ellipse at 50% 0%,#a44dba55,transparent 50%),
 radial-gradient(ellipse at 0% 100%,#ed78b833,transparent 45%),
 radial-gradient(ellipse at 100% 80%,#7958e744,transparent 45%),
 #10091e;
}
#birthdayLock.hidden{display:none}
.lock-orb{
 position:absolute;width:260px;height:260px;border-radius:50%;
 filter:blur(75px);opacity:.3;pointer-events:none;
 animation:orb 12s ease-in-out infinite alternate
}
.lock-orb.one{background:#ff65c8;top:-100px;left:-100px}
.lock-orb.two{background:#8963ff;right:-100px;bottom:-100px}
@keyframes orb{to{transform:translate(45px,-25px) scale(1.2)}}

.lock-card{
 position:relative;z-index:2;width:100%;max-width:490px;
 max-height:calc(100dvh - 32px);overflow-y:auto;
 text-align:center;padding:clamp(22px,5vw,34px);
 border:1px solid #ffd6f63d;border-radius:28px;
 background:linear-gradient(145deg,#30173de8,#160d2ae8);
 box-shadow:0 25px 100px #0008,0 0 45px #dc74ff16;
 backdrop-filter:blur(20px)
}
.lock-top,.eyebrow,.lock-date,.count-label{
 font:10px Arial,sans-serif;letter-spacing:2.5px;
 text-transform:uppercase;color:#edc9f1
}
.lock-heart{
 font-size:65px;line-height:1.3;color:#ff9edc;
 text-shadow:0 0 22px #ff6fc4;
 animation:heartBeat 1.8s infinite
}
@keyframes heartBeat{
 0%,100%{transform:scale(1)}
 12%,36%{transform:scale(1.1)}
 24%{transform:scale(1)}
}
.lock-title{
 font-size:clamp(40px,9vw,58px);font-weight:normal;
 line-height:1.05;margin:10px 0 14px
}
.lock-title span{
 display:block;color:var(--pink);
 text-shadow:0 0 30px #f67dd955
}
.lock-description{
 max-width:340px;margin:0 auto;color:#e5d5ee;
 font-size:15px;line-height:1.8
}
.divider{
 display:flex;justify-content:center;align-items:center;
 gap:12px;margin:22px;color:#ffd9f5
}
.divider i{
 width:42px;height:1px;
 background:linear-gradient(90deg,transparent,#f4a7e5,transparent)
}
.lock-date{margin-bottom:8px}
.birthday-date{font-size:22px;letter-spacing:5px;font-weight:normal;margin:0 0 20px}
#lockCountdown{
 display:grid;grid-template-columns:repeat(4,minmax(0,1fr));
 gap:8px;margin:12px 0 22px
}
.time-box{
 padding:13px 3px;border:1px solid #ffc8ee2c;
 background:#ffffff08;border-radius:13px
}
.time-box strong{
 display:block;font:clamp(22px,5vw,30px) Arial,sans-serif;
 color:#fff2ff;font-weight:normal;font-variant-numeric:tabular-nums
}
.time-box small{
 display:block;font:9px Arial,sans-serif;
 letter-spacing:1px;color:#d8b6e6;margin-top:6px
}

/* MUSIC PLAYER WORKS EVEN WHILE LOCKED */
.music-player{
 display:flex;align-items:center;gap:12px;text-align:left;
 padding:12px;border-radius:16px;border:1px solid #ffc7ec35;
 background:#ffffff0a
}
.music-art{
 width:44px;height:44px;flex-shrink:0;display:grid;place-items:center;
 border-radius:13px;background:linear-gradient(135deg,#ff9bd7,#9e81ff);
 color:#27112e;font-size:25px
}
.music-info{flex:1;min-width:0}
.music-info strong{display:block;font-size:13px;font-weight:normal}
.music-info span{display:block;font:10px Arial,sans-serif;color:#cdb5dc;margin-top:5px;overflow-wrap:anywhere}
.play-button{
 border:0;background:#ffb5e5;color:#29122d;border-radius:50%;
 width:42px;height:42px;flex-shrink:0;font-family:Arial,sans-serif
}
#musicStatus{font:11px Arial,sans-serif;color:#d8c0e5;min-height:15px;margin:10px 0 15px}
.lock-message{font-size:13px;color:#e8c9ef;line-height:1.6;font-style:italic}
.lock-footer{font:9px Arial,sans-serif;letter-spacing:2px;color:#bd9fcf;margin-top:22px}

/* MAIN WEBSITE */
#mainSite{position:relative;z-index:2}
nav{
 position:sticky;top:0;z-index:10;display:flex;gap:10px;
 align-items:center;justify-content:center;flex-wrap:wrap;
 padding:13px;background:#12091eea;border-bottom:1px solid #ffffff12;
 backdrop-filter:blur(15px)
}
nav a{font:11px Arial,sans-serif;color:#f0d8f3;padding:6px}
.brand{font-size:17px;color:var(--pink)}
.music-nav,.btn{
 display:inline-block;padding:12px 19px;border:1px solid #ffb9e577;
 border-radius:999px;color:#fff4ff;
 background:linear-gradient(120deg,#f18bc52b,#a88aff22);
 text-decoration:none;margin:5px
}
.hero{
 min-height:85vh;display:grid;place-items:center;text-align:center;
 padding:70px 20px;position:relative
}
.hero-inner{max-width:850px}
.kicker{font:11px Arial,sans-serif;letter-spacing:4px;color:var(--pink)}
.hero h1{font-size:clamp(46px,10vw,100px);font-weight:normal;line-height:1;margin:25px 0}
.hero h1 span{display:block;color:var(--pink)}
.hero p{max-width:600px;margin:25px auto;color:#e1cfe9;font-size:17px;line-height:1.8}
section{max-width:1050px;margin:auto;padding:60px 20px;scroll-margin-top:70px}
.heading{text-align:center;margin-bottom:28px}
.heading small{font:10px Arial,sans-serif;letter-spacing:3px;color:var(--pink)}
.heading h2{font-size:clamp(30px,6vw,46px);font-weight:normal;margin:12px 0}
.heading p{color:#d7c2e2;line-height:1.7}
.card{
 background:var(--glass);border:1px solid #ffffff20;
 border-radius:22px;padding:24px;backdrop-filter:blur(10px)
}
.center{text-align:center}
.note{font-size:17px;line-height:1.9;color:#f1dfef}
.grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(min(100%,220px),1fr));gap:15px}
.memory{padding:0;overflow:hidden}
.memory img,.memory video{width:100%;height:260px;object-fit:cover;display:block;background:#21122d}
.memory figcaption{padding:12px;font-size:13px;color:#e8d1ee}
.memory-placeholder{height:180px;display:grid;place-items:center;font-size:38px;color:var(--pink)}
.letter{
 max-width:750px;margin:auto;background:#fff0f8;color:#41254a;
 padding:clamp(24px,6vw,45px);border-radius:8px;line-height:1.9
}
.letter h3{text-align:center;font-size:30px;font-weight:normal;color:#9d4586}
.gift{width:100%;min-height:130px;border:1px solid #ffb6e533;background:#ffffff08;border-radius:17px;color:white;padding:18px}
.gift span{display:block;font-size:32px;margin-bottom:10px}
.result{color:#ffc5e9;line-height:1.7;min-height:24px}
footer{text-align:center;padding:45px 15px;color:#bda3ce;font:10px Arial,sans-serif;letter-spacing:2px}
@media(max-width:600px){
 nav{gap:3px;padding:8px 5px}nav a{font-size:10px;padding:5px}
 .brand{width:100%;text-align:center}
 .hero{min-height:75vh}
 .hero p{font-size:15px}
 .memory img,.memory video{height:230px}
 .lock-card{border-radius:23px}
}
@media(prefers-reduced-motion:reduce){
 *,*:before,*:after{animation-duration:.01ms!important;scroll-behavior:auto!important}
}
</style>
</head>

<body>
<div id="siteMagic"></div>

<!-- BEAUTIFUL LOCK SCREEN -->
<div id="birthdayLock">
 <div id="lockMagic"></div>
 <div class="lock-orb one"></div><div class="lock-orb two"></div>

 <div class="lock-card">
  <div class="lock-top">✦ A LITTLE UNIVERSE MADE FOR YOU ✦</div>
  <div class="lock-heart">♡</div>
  <p class="eyebrow">Someone special is waiting for a special day</p>
  <h1 class="lock-title">For <span>Khusssss</span></h1>
  <p class="lock-description">A thousand little stars, a million little wishes, and all my love are waiting here just for you.</p>
  <div class="divider"><span>✧</span><i></i><span>♡</span><i></i><span>✧</span></div>
  <p class="lock-date">YOUR MAGIC DAY</p>
  <h2 class="birthday-date">04 · 06 · 2027</h2>
  <div class="count-label">YOUR BIRTHDAY BEGINS IN</div>
  <div id="lockCountdown">
   <div class="time-box"><strong id="days">000</strong><small>DAYS</small></div>
   <div class="time-box"><strong id="hours">00</strong><small>HOURS</small></div>
   <div class="time-box"><strong id="minutes">00</strong><small>MINS</small></div>
   <div class="time-box"><strong id="seconds">00</strong><small>SECS</small></div>
  </div>

  <div class="music-player">
   <div class="music-art">♫</div>
   <div class="music-info"><strong>A little song for you</strong><span>Song22.mp3 · Birthday soundtrack</span></div>
   <button class="play-button" id="lockPlay" aria-label="Play or pause song">▶</button>
  </div>
  <p id="musicStatus">Tap play to listen before the birthday ♡</p>
  <p class="lock-message">Your birthday universe is waiting to bloom. ✧</p>
  <div class="lock-footer">MADE WITH LOVE · FOREVER YOURS ♡</div>
 </div>
</div>

<!-- Keep this audio element outside the lock so the song works before and after unlock. -->
<audio id="birthdaySong" src="Song22.mp3" loop preload="metadata"></audio>

<!-- MAIN WEBSITE: shown automatically on 4 June 2027 -->
<div id="mainSite" class="hidden">
 <nav>
  <span class="brand">♡ Khusssss</span>
  <a href="#home">Home</a><a href="#memories">Memories</a><a href="#letter">Letter</a><a href="#gifts">Gifts</a><a href="#games">Fun</a>
  <button class="music-nav" id="mainPlay">♫ Music</button>
 </nav>

 <header class="hero" id="home">
  <div class="hero-inner">
   <div class="kicker">✦ TODAY, THE UNIVERSE CELEBRATES YOU ✦</div>
   <h1>Happy Birthday <span>Khusssss</span></h1>
   <p>This little universe is made of memories, tiny surprises, warm wishes, and a whole lot of love. Every star here is cheering for you.</p>
   <a class="btn" href="#letter">Open your letter ♡</a>
   <a class="btn" href="#gifts">Explore your surprises ✧</a>
  </div>
 </header>

 <section>
  <div class="heading"><small>A LITTLE REMINDER</small><h2>You Are So Loved</h2></div>
  <div class="card center note">Khusssss, I hope this new year of your life brings you peace when you need it, courage when things feel difficult, laughter that makes your cheeks hurt, and beautiful moments you will remember forever. Never forget how special you are. ♡</div>
 </section>

 <section id="memories">
  <div class="heading"><small>LITTLE PIECES OF FOREVER</small><h2>Our Memory Gallery</h2><p>Photos K1.jpg to K10.jpg and K12.jpg, plus video K11.mp4.</p></div>
  <div class="grid" id="gallery"></div>
 </section>

 <section>
  <div class="heading"><small>A STORY STILL BEING WRITTEN</small><h2>Our Little Timeline</h2></div>
  <div class="grid">
   <div class="card"><h3>🌷 The beginning</h3><p>Every lovely story has a first page. This is one I will always be glad to have.</p></div>
   <div class="card"><h3>✨ The little moments</h3><p>The laughs, the conversations, the silly things, and the memories that quietly matter most.</p></div>
   <div class="card"><h3>🌙 Everything to come</h3><p>More adventures, more smiles, more photographs, and more reasons to celebrate you.</p></div>
  </div>
 </section>

 <section id="letter">
  <div class="heading"><small>OPEN WHEN YOU NEED A SMILE</small><h2>A Letter For You</h2></div>
  <div class="letter">
   <h3>Dear Khusssss ♡</h3>
   <p>Happy Birthday to someone who deserves all the beautiful things this world can offer.</p>
   <p>I made this little website so you could have a place full of stars, memories, and reminders that you matter. It may be made from code, but every little detail is here to make your day feel special.</p>
   <p>I hope you keep choosing happiness, keep believing in yourself, and never stop dreaming big. May your heart feel lighter, your days feel brighter, and your future bring you more than you ever expected.</p>
   <p>Whenever you visit this page, remember: you are appreciated, you are important, and you deserve to be celebrated—not just today, but all year long.</p>
   <p style="text-align:right">With lots of love,<br><strong>Always ♡</strong></p>
  </div>
 </section>

 <section id="gifts">
  <div class="heading"><small>A FEW TINY TREASURES</small><h2>Your Surprise Boxes</h2><p>Tap a box to reveal its message.</p></div>
  <div class="grid">
   <button class="gift" data-message="May good news find you, kind people stay near you, and happy moments surprise you."><span>🎁</span>Gift 01<br><small>A little surprise</small></button>
   <button class="gift" data-message="May you trust yourself enough to begin, and be proud of yourself for trying."><span>💌</span>Gift 02<br><small>A note just for you</small></button>
   <button class="gift" data-message="May your days be full of jokes, unforgettable stories, and people who make you feel at home."><span>🌷</span>Gift 03<br><small>A flower made of words</small></button>
   <button class="gift" data-message="May the things you work for slowly become the life you once imagined."><span>🌟</span>Gift 04<br><small>A star for your future</small></button>
   <button class="gift" data-message="May you rest without guilt, breathe without worry, and remember you do not have to do everything at once."><span>🌙</span>Gift 05<br><small>A little calm</small></button>
   <button class="gift" data-message="May you always be surrounded by people who respect your heart and celebrate the real you."><span>💗</span>Gift 06<br><small>A heartful wish</small></button>
   <button class="gift" data-message="May this be a year of new chapters, brave choices, good health, and moments that make you glad to be alive."><span>🗝️</span>Gift 07<br><small>The final treasure</small></button>
  </div>
  <div class="card center" style="margin-top:15px"><p id="giftResult" class="result">Your surprise will appear here ♡</p></div>
 </section>

 <section id="games">
  <div class="heading"><small>A TINY BIRTHDAY PLAYGROUND</small><h2>Let's Have Some Fun</h2></div>
  <div class="grid">
   <div class="card center"><div style="font-size:48px" id="cake">🎂</div><h3>Make a Wish</h3><p>Make a wish and blow out the virtual candle.</p><button class="btn" id="blowCandle">Blow the candle ✨</button><p class="result" id="candleResult"></p></div>
   <div class="card center"><div style="font-size:42px">💗</div><h3>Sister Quiz</h3><p>What does your birthday deserve most?</p><button class="btn quiz">Happiness</button><button class="btn quiz">Adventure</button><button class="btn quiz">Love</button><p class="result" id="quizResult"></p></div>
   <div class="card center"><div style="font-size:42px">🔮</div><h3>Future Fortune</h3><p>Tap to reveal a tiny prediction.</p><button class="btn" id="fortune">Reveal my fortune</button><p class="result" id="fortuneResult"></p></div>
   <div class="card center"><div style="font-size:42px">🫂</div><h3>Virtual Hug</h3><p>A little warmth through the screen.</p><button class="btn" id="hug">Send a hug ♡</button><p class="result" id="hugResult"></p></div>
  </div>
 </section>

 <section id="wishes">
  <div class="heading"><small>PUT A LITTLE HOPE INTO THE UNIVERSE</small><h2>The Wish Jar</h2></div>
  <div class="card center"><div style="font-size:60px">🏺</div>
   <form id="wishForm"><input id="wishInput" maxlength="180" required placeholder="Write a wish for this new year..." style="width:min(100%,480px);padding:13px;border-radius:12px;border:1px solid #ffffff25;background:#130b20;color:white"><button class="btn">Add my wish ✧</button></form>
   <p class="result" id="wishResult"></p><div id="wishWall"></div>
  </div>
 </section>

 <section id="reasons">
  <div class="heading"><small>A FEW REMINDERS</small><h2>Reasons You Are Wonderful</h2></div>
  <div class="card center"><div id="reasonNumber" style="font-size:45px;color:var(--pink)">01</div><p class="note" id="reasonText">Your presence can make an ordinary day feel special.</p><button class="btn" id="nextReason">Another reason ♡</button><p id="reasonCounter" class="result">1 OF 50</p></div>
 </section>

 <section>
  <div class="heading"><small>A GARDEN THAT NEVER FADES</small><h2>Birthday Garden</h2></div>
  <div class="card center"><div id="flowers" style="font-size:35px;line-height:1.9">🌱</div><button class="btn" id="growFlower">Plant a flower 🌷</button><p class="result" id="flowerResult">Your garden is ready to grow.</p></div>
 </section>

 <section>
  <div class="heading"><small>ONE LAST THING</small><h2>Your Universe, Always</h2></div>
  <div class="card center"><div style="font-size:65px">🌌</div><p class="note">Somewhere in this huge universe, there is a little page made especially to celebrate you.</p><button class="btn" id="finale">Fill the sky with stars ✨</button><p class="result" id="finaleResult"></p></div>
 </section>

 <footer>MADE WITH LOVE FOR KHUSSSSS · HAPPY BIRTHDAY ♡</footer>
</div>

<script>
(() => {
 const birthday = new Date("2027-06-04T00:00:00+05:30");
 const lock = document.getElementById("birthdayLock");
 const main = document.getElementById("mainSite");
 const song = document.getElementById("birthdaySong");
 const status = document.getElementById("musicStatus");
 const lockPlay = document.getElementById("lockPlay");
 const mainPlay = document.getElementById("mainPlay");

 // Music is NOT tied to the countdown or lock. It works at all times.
 async function toggleMusic() {
   try {
     if (song.paused) {
       await song.play();
       status.textContent = "Playing your birthday song ♡";
     } else {
       song.pause();
       status.textContent = "Paused — play whenever you like ♡";
     }
   } catch (e) {
     status.textContent = "Please upload Song22.mp3 beside index.html.";
   }
 }
 lockPlay.addEventListener("click", toggleMusic);
 mainPlay.addEventListener("click", toggleMusic);
 function updateMusicButtons() {
   const playing = !song.paused;
   lockPlay.textContent = playing ? "Ⅱ" : "▶";
   mainPlay.textContent = playing ? "♫ Pause" : "♫ Music";
 }
 song.addEventListener("play", updateMusicButtons);
 song.addEventListener("pause", updateMusicButtons);
 song.addEventListener("error", () => status.textContent = "Song22.mp3 not found. Check the filename and folder.");

 function unlock() {
   lock.classList.add("hidden");
   main.classList.remove("hidden");
 }
 function countdown() {
   const diff = birthday.getTime() - Date.now();
   if (diff <= 0) {
     unlock();
     return;
   }
   const total = Math.floor(diff / 1000);
   document.getElementById("days").textContent = String(Math.floor(total / 86400)).padStart(3,"0");
   document.getElementById("hours").textContent = String(Math.floor(total % 86400 / 3600)).padStart(2,"0");
   document.getElementById("minutes").textContent = String(Math.floor(total % 3600 / 60)).padStart(2,"0");
   document.getElementById("seconds").textContent = String(total % 60).padStart(2,"0");
 }
 countdown();
 setInterval(countdown,1000);

 // Hearts and sparkles continue on the lock screen and main site.
 function particle(layer) {
   const p = document.createElement("span");
   p.className = "particle";
   p.textContent = ["♡","♥","✦","✧","⋆","✨","·"][Math.floor(Math.random()*7)];
   p.style.left = Math.random()*100 + "%";
   p.style.fontSize = (12 + Math.random()*18) + "px";
   p.style.animationDuration = (8 + Math.random()*9) + "s";
   p.style.color = ["#ffb9e7","#e2c9ff","#fff0c8","#ff8dcf"][Math.floor(Math.random()*4)];
   layer.appendChild(p);
   setTimeout(() => p.remove(),18000);
 }
 const lockMagic = document.getElementById("lockMagic");
 const siteMagic = document.getElementById("siteMagic");
 setInterval(() => particle(lockMagic),300);
 setInterval(() => { if (!main.classList.contains("hidden")) particle(siteMagic); },400);

 // Gallery media names match the files in the repository.
 const gallery = document.getElementById("gallery");
 const captions = ["A favourite little moment","A memory worth keeping","A page in our story","A smile to remember","One for the scrapbook","A little bit of forever","A moment full of warmth","Another lovely memory","A picture full of meaning","A little treasure","The final memory"];
 [...Array(10)].map((_,i)=>i+1).concat([12]).forEach(n => {
   const fig = document.createElement("figure");
   fig.className = "card memory";
   const img = document.createElement("img");
   img.src = `K${n}.jpg`;
   img.alt = captions[n-1] || "Birthday memory";
   img.loading = "lazy";
   img.onerror = () => { fig.innerHTML = `<div class="memory-placeholder">♡</div><figcaption>Upload K${n}.jpg to show this memory</figcaption>`; };
   const cap = document.createElement("figcaption");
   cap.textContent = captions[n-1] || "A little memory";
   fig.append(img,cap); gallery.appendChild(fig);
 });
 const video = document.createElement("figure");
 video.className = "card memory";
 video.innerHTML = '<video src="K11.mp4" controls preload="metadata"></video><figcaption>A moving memory — K11.mp4</figcaption>';
 gallery.appendChild(video);

 document.querySelectorAll(".gift").forEach(b => b.addEventListener("click", () => {
   document.getElementById("giftResult").textContent = b.dataset.message;
 }));
 document.getElementById("blowCandle").addEventListener("click", () => {
   document.getElementById("cake").textContent = "🍰";
   document.getElementById("candleResult").textContent = "Wish sent to the universe. May it find its way to you. ♡";
 });
 document.querySelectorAll(".quiz").forEach(b => b.addEventListener("click", () => {
   document.getElementById("quizResult").textContent = "Correct answer: ALL OF THEM. You deserve every good thing. ♡";
 }));
 const fortunes = [
   "A lovely surprise may be closer than you think. ✨",
   "You will find a reason to be proud of yourself.",
   "A new memory is waiting to be made.",
   "Keep going—your effort matters more than you know.",
   "May the right doors open at the right time. ♡"
 ];
 document.getElementById("fortune").addEventListener("click", () => {
   document.getElementById("fortuneResult").textContent = fortunes[Math.floor(Math.random()*fortunes.length)];
 });
 document.getElementById("hug").addEventListener("click", () => {
   document.getElementById("hugResult").textContent = "♡ ♡ ♡ A giant virtual hug, wrapped in sparkles, is on its way! ♡ ♡ ♡";
 });
 document.getElementById("wishForm").addEventListener("submit", e => {
   e.preventDefault();
   const input = document.getElementById("wishInput");
   const value = input.value.trim();
   if (!value) return;
   const item = document.createElement("div");
   item.textContent = "✧ " + value;
   item.style.cssText = "padding:12px;margin:9px 0;border-radius:12px;background:#ffffff0a;border:1px solid #ffffff12";
   document.getElementById("wishWall").prepend(item);
   document.getElementById("wishResult").textContent = "Your wish has been placed in the jar. ♡";
   input.value = "";
 });
 const reasons = [
  "Your presence can make an ordinary day feel special.","You deserve kindness even on difficult days.","Your laugh can brighten a room.","You are allowed to grow at your own pace.","Your dreams are worth taking seriously.",
  "You have your own special way of seeing the world.","You can begin again whenever you need to.","Your feelings deserve to be heard.","You bring something unique to the people around you.","You deserve rest as much as success.",
  "You are more than one bad day.","Your future is full of possibilities.","You can be brave and nervous at the same time.","You deserve people who celebrate your wins.","Your little efforts count.",
  "You make memories that matter.","You are worthy of respect.","Your kindness is valuable.","You do not need to be perfect to be loved.","You deserve to feel proud of yourself.",
  "You can learn from mistakes without becoming them.","Your ideas deserve space.","You can take life one step at a time.","Your smile is worth protecting.","You deserve safe and sincere friendships.",
  "You can change your mind and keep growing.","You are allowed to ask for help.","Your story is still unfolding.","You have survived difficult days.","Your hopes are worth nurturing.",
  "You deserve joy without having to earn it.","You can make a fresh start.","Your voice matters.","You have so much left to discover.","You deserve love that feels peaceful.",
  "You can make small things beautiful.","Your curiosity can take you places.","You are not behind in your own story.","You can be proud of progress, not just results.","Your heart deserves gentleness.",
  "You can choose what helps you grow.","You deserve to be listened to.","You have the power to make new memories.","Your presence matters more than you know.","You can be both strong and soft.",
  "You deserve good surprises.","You are capable of learning new things.","There are still so many beautiful days ahead.","You are loved in ways you may not always see.","The world is better with your own kind of sparkle. ♡"
 ];
 let reasonIndex = 0;
 document.getElementById("nextReason").addEventListener("click", () => {
   reasonIndex = (reasonIndex + 1) % reasons.length;
   document.getElementById("reasonNumber").textContent = String(reasonIndex+1).padStart(2,"0");
   document.getElementById("reasonText").textContent = reasons[reasonIndex];
   document.getElementById("reasonCounter").textContent = `${reasonIndex+1} OF ${reasons.length}`;
 });
 let flowerCount = 0;
 const flowers = ["🌷","🌸","🌼","🌻","💐","🌺","🪻"];
 document.getElementById("growFlower").addEventListener("click", () => {
   flowerCount++;
   document.getElementById("flowers").textContent += " " + flowers[(flowerCount-1)%flowers.length];
   document.getElementById("flowerResult").textContent = `${flowerCount} little flower${flowerCount===1?" has":"s have"} grown from your wishes.`;
 });
 document.getElementById("finale").addEventListener("click", () => {
   for(let i=0;i<45;i++) setTimeout(()=>particle(main.classList.contains("hidden")?lockMagic:siteMagic),i*35);
   document.getElementById("finaleResult").textContent = "The sky is full of stars, and every one sends you a little wish. Happy Birthday, Khusssss! ♡";
 });
})();
</script>
</body>
</html>
