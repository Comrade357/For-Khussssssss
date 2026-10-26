
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<meta name="theme-color" content="#10091b">
<title>For Khusssss ♡</title>

<style>
:root {
  --bg:#10091b; --pink:#ff8ecb; --purple:#bd9aff;
  --gold:#ffe1a8; --text:#fff3fb; --muted:#d5c4dc;
}
* { box-sizing:border-box; }
html { scroll-behavior:smooth; }
body {
  margin:0; color:var(--text);
  font-family:Georgia,"Times New Roman",serif;
  background:radial-gradient(ellipse at top,#3a1745,transparent 55%),
  radial-gradient(ellipse at bottom right,#29113d,transparent 45%),var(--bg);
  overflow-x:hidden;
}
button {
  font:inherit; cursor:pointer; padding:12px 18px; border-radius:30px;
  border:1px solid #ffb4e059;
  background:linear-gradient(135deg,var(--pink),var(--purple));
  color:#28112e; font-weight:bold; transition:.25s;
}
button:hover { transform:translateY(-2px); filter:brightness(1.08); }
button.secondary { background:#ffffff0c; color:var(--text); }
a { color:var(--pink); text-decoration:none; }
.hidden { display:none!important; }
section { padding:60px 17px; scroll-margin-top:80px; }
.wrap { max-width:1000px; margin:auto; }
.center { text-align:center; }
h1,h2,h3 { line-height:1.25; }
h1 { font-size:clamp(38px,8vw,72px); margin:15px 0; }
h2 { font-size:clamp(28px,5vw,42px); }
h3 { color:#ffd0e9; }
p { color:var(--muted); line-height:1.85; }
.eyebrow { color:var(--pink); font-size:11px; letter-spacing:3px; text-transform:uppercase; }
.gradient {
  background:linear-gradient(100deg,#ff9ed4,#d4b3ff,#ffe1a8);
  color:transparent; background-clip:text; -webkit-background-clip:text;
}
.card {
  padding:23px; border-radius:22px; background:#ffffff09;
  border:1px solid #ffb4e027; box-shadow:0 12px 35px #0002;
  backdrop-filter:blur(10px);
}
.grid { display:grid; grid-template-columns:repeat(auto-fit,minmax(min(100%,230px),1fr)); gap:15px; }
.pill { display:inline-block; border:1px solid #ff8ecb35; background:#ff8ecb15; border-radius:30px; padding:7px 12px; font-size:12px; }
.small-note { color:#bba8c8; font-size:12px; }
hr { border:0; border-top:1px solid #ffffff18; margin:22px 0; }
#particles { position:fixed; inset:0; pointer-events:none; overflow:hidden; z-index:10; }
.particle { position:absolute; bottom:-30px; animation:floatUp linear forwards; text-shadow:0 0 12px #ff8ecb; }
@keyframes floatUp { to { transform:translateY(-115vh) rotate(300deg); opacity:0; } }
@keyframes pulse { 50% { transform:scale(1.05); } }
@keyframes reveal { from {opacity:0;transform:translateY(12px)} to {opacity:1;transform:translateY(0)} }

#birthdayLock {
  min-height:100svh; display:flex; align-items:center; justify-content:center;
  padding:24px 15px; position:relative; z-index:2;
}
.lock-card {
  width:min(720px,100%); text-align:center; padding:clamp(22px,5vw,48px);
  background:#12091eeb; border:1px solid #ffb9e83c; border-radius:30px;
  box-shadow:0 0 80px #d65bb21c;
}
.lock-icon { font-size:48px; color:#ffb7e0; animation:pulse 3s infinite; }
.countdown { display:grid; grid-template-columns:repeat(4,minmax(0,1fr)); gap:8px; margin:24px 0; }
.timebox { background:#ffffff0a; border:1px solid #ffffff16; padding:14px 3px; border-radius:14px; }
.timebox strong { display:block; font-size:clamp(23px,6vw,35px); color:#ffb7e0; }
.timebox span { font-size:10px; color:var(--muted); letter-spacing:1px; }

.daily-quote-card {
  margin:24px 0; padding:22px 18px; border-radius:22px;
  background:linear-gradient(145deg,#ff8ecb18,#bd9aff18);
  border:1px solid #ffb4e04d; box-shadow:0 0 35px #ff8ecb10;
  animation:reveal 1s ease both;
}
.daily-quote-label { color:#ffabd9; font-size:10px; letter-spacing:2px; margin-bottom:15px; }
.daily-quote-heading { color:#e4caff; font-size:14px; margin-bottom:12px; }
#dailyQuote { min-height:85px; display:grid; place-items:center; color:#fff0fa; font-size:clamp(18px,4vw,23px); line-height:1.7; font-style:italic; }
#dailyQuoteDate { color:#ffabd9; font-size:12px; margin-top:14px; }
.daily-quote-footer { color:#c9b7d7; font-size:11px; margin-top:15px; }

.music-panel { margin-top:20px; padding:17px; border-radius:18px; background:#ffffff09; border:1px solid #ffffff17; }
nav { position:sticky; top:0; z-index:5; background:#10091bee; backdrop-filter:blur(15px); border-bottom:1px solid #ffffff16; }
.nav-inner { max-width:1000px; margin:auto; padding:12px; display:flex; align-items:center; justify-content:space-between; gap:10px; }
.brand { color:#ffd0e9; font-weight:bold; white-space:nowrap; }
.nav-links { display:flex; gap:8px; flex-wrap:wrap; justify-content:center; }
.nav-links a { color:#e8d9ee; font-size:12px; padding:5px; }
.nav-links a:hover { color:var(--pink); }
.hero { min-height:75vh; display:grid; place-items:center; text-align:center; padding:60px 20px; }
.hero-inner { max-width:800px; animation:reveal 1s both; }
.hero-heart { font-size:44px; color:#ffb7e0; animation:pulse 3s infinite; }
.quote-mark { font-size:35px; color:var(--pink); }
.quote-text { font-size:clamp(19px,4vw,25px); line-height:1.8; color:#ffe5f4; }
.quote-author { color:var(--pink); font-size:13px; }
.photo { width:100%; height:205px; object-fit:cover; border-radius:14px; background:#24152f; }
.memory-card { overflow:hidden; }
.reason { padding:13px; border-radius:14px; background:#ffffff08; border:1px solid #ffffff12; color:#f8d8ed; line-height:1.7; }
.reason b { color:var(--pink); margin-right:7px; }
.big-number { font-size:40px; color:var(--pink); }
.letter { white-space:pre-line; line-height:2; color:#f6dfee; }
.message-box { min-height:100px; display:grid; place-items:center; text-align:center; line-height:1.9; color:#ffe3f3; font-size:18px; }
#quoteSearch { width:100%; margin:10px 0 20px; padding:13px 17px; border-radius:25px; background:#ffffff09; color:white; border:1px solid #ffffff22; font:inherit; }
#quoteSearch::placeholder { color:#bba8c8; }
#quoteCounter { font-size:12px; }
#garden { min-height:100px; display:flex; flex-wrap:wrap; justify-content:center; align-items:center; gap:10px; font-size:30px; }
footer { text-align:center; padding:40px 15px; border-top:1px solid #ffffff12; }
#toast { display:none; position:fixed; z-index:20; bottom:20px; left:50%; transform:translateX(-50%); width:max-content; max-width:90%; padding:13px 18px; border-radius:15px; background:#2a1738; color:#fff1fa; border:1px solid #ff9ed455; }
#toast.show { display:block; animation:reveal .3s both; }
@media(max-width:600px) {
  .nav-inner { flex-direction:column; }
  .nav-links { gap:3px; }
  .nav-links a { font-size:11px; }
  section { padding:45px 14px; }
  .card { padding:18px; }
}
@media(prefers-reduced-motion:reduce) { *,*::before,*::after { animation-duration:.01ms!important; scroll-behavior:auto!important; } }
</style>
</head>

<body>
<div id="particles" aria-hidden="true"></div>

<!-- Keep the song outside the locked section so it can play before and after the birthday. -->
<audio id="birthdaySong" src="Song22.mp3" loop preload="metadata"></audio>

<div id="birthdayLock">
  <div class="lock-card">
    <div class="lock-icon">♡</div>
    <div class="eyebrow">A little universe made for you</div>
    <h1 class="gradient">For Khusssss</h1>
    <p>A special little world made with love, just for you 💗                                            Sending you warm wishes ahead of time so the celebration lasts longer. Happy advance birthday! Counting down the days to your special day. Happy early birthday, sister!✨💙.</p>

    <div class="pill">Your birthday countdown ✧</div>
    <div class="countdown" id="countdown">
      <div class="timebox"><strong id="days">000</strong><span>DAYS</span></div>
      <div class="timebox"><strong id="hours">00</strong><span>HOURS</span></div>
      <div class="timebox"><strong id="minutes">00</strong><span>MINUTES</span></div>
      <div class="timebox"><strong id="seconds">00</strong><span>SECONDS</span></div>
    </div>
    <p id="lockMessage">Your birthday world opens on 4 June 2027. ♡</p>

    <!-- DAILY MOTIVATIONAL QUOTE -->
    <div class="daily-quote-card">
      <div class="daily-quote-label">✧ YOUR DAILY DOSE OF INSPIRATION ✧</div>
      <div class="daily-quote-heading">A little reminder for your future</div>
      <div id="dailyQuote">Your future is built by the little things you do today.</div>
      <div id="dailyQuoteDate"></div>
      <div class="daily-quote-footer">One day. One thought. One step forward. ♡</div>
    </div>

    <div class="music-panel">
      <div class="eyebrow">Your little soundtrack</div>
      <p>A song for you, whenever you want to listen.</p>
      <button id="lockPlay" onclick="toggleMusic()">▶ Play Song</button>
      <p class="small-note">Tap to start the music. Browsers usually require a user tap.</p>
    </div>
  </div>
</div>

<div id="mainSite" class="hidden">
  <nav>
    <div class="nav-inner">
      <div class="brand">♡ For Khusssss</div>
      <div class="nav-links">
        <a href="#home">Home</a><a href="#wishes">Wishes</a>
        <a href="#quotes">Quotes</a><a href="#memories">Memories</a>
        <a href="#letter">Letter</a><a href="#reasons">Reasons</a>
        <a href="#surprises">Surprises</a>
      </div>
    </div>
  </nav>

  <header class="hero" id="home">
    <div class="hero-inner">
      <div class="hero-heart">♡ ✧ ♡</div>
      <div class="eyebrow">4 June 2027 · Your day · Your universe</div>
      <h1>Happy Birthday,<br><span class="gradient">Khusssss</span></h1>
      <p style="font-size:18px">To my sister, my forever family, and one of the sweetest blessings in life. This little universe is yours.</p>
      <p><a href="#letter"><button>Read Your Letter ♡</button></a> <a href="#quotes"><button class="secondary">Sister Quotes ✧</button></a></p>
    </div>
  </header>

  <section id="wishes">
    <div class="wrap">
      <div class="center"><div class="eyebrow">Thirty little wishes</div><h2>30 Wishes for <span class="gradient">My Sister</span></h2><p>Every wish is a reminder that you deserve good things.</p></div>
      <div class="grid" id="wishGrid"></div>
    </div>
  </section>

  <section id="quotes">
    <div class="wrap">
      <div class="center"><div class="eyebrow">Words from the heart</div><h2>Our <span class="gradient">Sisterhood Library</span></h2><p>100 sister quotes to read, save, and share.</p></div>
      <div class="card center" style="margin-bottom:24px">
        <div class="quote-mark">“</div><div class="message-box" id="randomQuote">A sister is a little piece of home you can carry everywhere.</div>
        <p class="quote-author" id="quoteAuthor">A note from the heart</p><p id="quoteCounter">Quote 1 of 100</p>
        <button onclick="newQuote()">New Quote ✧</button> <button class="secondary" onclick="copyQuote()">Copy Quote</button>
      </div>
      <input id="quoteSearch" type="text" placeholder="Search sister quotes..." aria-label="Search sister quotes">
      <div class="grid" id="quoteGrid"></div>
      <div class="center" style="margin-top:22px"><button class="secondary" id="moreQuotes" onclick="showMoreQuotes()">Show More Quotes</button></div>
    </div>
  </section>

  <section id="memories">
    <div class="wrap">
      <div class="center"><div class="eyebrow">Little pieces of our story</div><h2>Our <span class="gradient">Memory Gallery</span></h2><p>Upload the matching photos and video to the same folder as this page.</p></div>
      <div class="grid" id="gallery"></div>
    </div>
  </section>

  <section id="timeline">
    <div class="wrap">
      <div class="center"><div class="eyebrow">A bond that keeps growing</div><h2>A Little <span class="gradient">Sister Timeline</span></h2></div>
      <div class="grid">
        <div class="card"><span class="pill">Chapter 01</span><h3>Where it begins</h3><p>A family, a bond, and a connection special in its own way.</p></div>
        <div class="card"><span class="pill">Chapter 02</span><h3>The little moments</h3><p>Conversations, laughter, and memories that make life warmer.</p></div>
        <div class="card"><span class="pill">Chapter 03</span><h3>Growing together</h3><p>Different dreams, new experiences, and a bond that continues to matter.</p></div>
        <div class="card"><span class="pill">Chapter 04</span><h3>Always family</h3><p>Wherever life takes us, you will always have a place in my heart.</p></div>
      </div>
    </div>
  </section>

  <section id="letter">
    <div class="wrap">
      <div class="center"><div class="eyebrow">Please read this slowly</div><h2>A Letter <span class="gradient">Just for You</span></h2></div>
      <div class="card">
        <p class="letter">Dear Khusssss,

Happy Birthday to one of the most special people in my life.

I hope you know that you are loved for much more than the things you do. You are valuable simply because you are you. You do not have to be perfect or have every part of life figured out to deserve happiness.

I wish you a life filled with peaceful mornings, genuine smiles, beautiful surprises, meaningful friendships, and dreams that slowly become real. When life gets difficult, I hope you remember how strong you are. When you feel uncertain, give yourself the same patience you would give someone you love.

Thank you for being my sister. No birthday message could ever explain every little thing that makes our bond special. I hope this website reminds you that someone took time to make something just for you, because you matter.

Keep smiling, keep dreaming, and keep being your own beautiful self. May the world give you more reasons to laugh than reasons to worry.

No matter how much life changes, I hope we always find our way back to laughter, care, and family.

Happy Birthday, Khusssss. May this new year of your life be gentle with your heart and generous with your dreams.

With lots of love,
Your sibling ♡</p>
        <hr><p class="center">“You will never need to earn your place in my heart. You already have one.”</p>
      </div>
    </div>
  </section>

  <section id="reasons">
    <div class="wrap">
      <div class="center"><div class="eyebrow">A hundred little reminders</div><h2>100 Reasons <span class="gradient">You're Special</span></h2><p>Little reminders of how much a sister can mean.</p></div>
      <div class="grid" id="reasonGrid"></div>
    </div>
  </section>

  <section id="promises">
    <div class="wrap">
      <div class="center"><div class="eyebrow">A promise from the heart</div><h2>Things I Hope <span class="gradient">You Always Know</span></h2></div>
      <div class="grid">
        <div class="card"><h3>♡ You can be yourself</h3><p>You don't have to pretend to be strong every second. Your feelings matter.</p></div>
        <div class="card"><h3>♡ Your dreams matter</h3><p>Your ambitions deserve room to grow, even when the path takes time.</p></div>
        <div class="card"><h3>♡ You deserve respect</h3><p>You deserve people who listen, care, and treat you with kindness.</p></div>
        <div class="card"><h3>♡ You are not alone</h3><p>Asking for support is a strength, not a weakness.</p></div>
        <div class="card"><h3>♡ Keep your own light</h3><p>You never need to become someone else to be worthy of love.</p></div>
        <div class="card"><h3>♡ You are loved</h3><p>Ordinary days are better because you are part of our family.</p></div>
      </div>
    </div>
  </section>

  <section id="surprises">
    <div class="wrap">
      <div class="center"><div class="eyebrow">Tap, discover, smile</div><h2>Little <span class="gradient">Birthday Surprises</span></h2><p>Every button hides a little something for you.</p></div>
      <div class="grid">
        <div class="card center"><div class="big-number">01</div><h3>A secret message</h3><p id="secretMessage">There's something waiting here.</p><button onclick="revealSecret()">Reveal Message ♡</button></div>
        <div class="card center"><div class="big-number">02</div><h3>A virtual hug</h3><p id="hugMessage">Ready for a little hug?</p><button onclick="virtualHug()">Send a Hug</button></div>
        <div class="card center"><div class="big-number">03</div><h3>Your birthday fortune</h3><p id="fortuneMessage">Your next surprise is waiting.</p><button onclick="fortune()">Read Your Fortune ✨</button></div>
        <div class="card center"><div class="big-number">04</div><h3>Make a wish</h3><p>Think of a wish, then add a flower to your garden.</p><button onclick="plantFlower()">Plant a Flower</button></div>
      </div>
      <div class="card center" style="margin-top:20px"><h3>Your Birthday Garden</h3><p>Every flower represents a wish for your happiness.</p><div id="garden"><span class="small-note">Your garden is waiting for its first flower.</span></div><p id="flowerCount">Flowers planted: 0</p></div>
    </div>
  </section>

  <section id="finale">
    <div class="wrap center">
      <div class="hero-heart">♡ ✧ ♡</div><div class="eyebrow">One last thing</div><h2>You Will Always Be <span class="gradient">Special</span></h2>
      <div class="card"><p class="quote-text">“The world may change, years may pass, and life may take us in different directions. But the love we have for our family will always be a beautiful part of who we are.”</p><p>Happy Birthday, Khusssss. Keep this little universe close to your heart. ♡</p><button onclick="celebrate()">Celebrate Again ✨</button></div>
      <div class="music-panel"><p>Want to listen to your song again?</p><button id="mainPlay" onclick="toggleMusic()">▶ Play Song</button></div>
    </div>
  </section>

  <footer><div class="hero-heart">♡</div><p>Made with love for Khusssss</p><p>4 June 2027 · A little universe, made just for you.</p></footer>
</div>

<div id="toast" role="status" aria-live="polite"></div>

<script>
"use strict";

/* COUNTDOWN: JUNE 4, 2027 AT MIDNIGHT INDIA TIME */
const birthday = new Date("2027-06-04T00:00:00+05:30");
let unlocked = false;
const audio = document.getElementById("birthdaySong");

function updateCountdown() {
  const remaining = birthday.getTime() - Date.now();
  if (remaining <= 0) { unlockBirthday(); return; }

  const total = Math.floor(remaining / 1000);
  document.getElementById("days").textContent = String(Math.floor(total / 86400)).padStart(3,"0");
  document.getElementById("hours").textContent = String(Math.floor(total % 86400 / 3600)).padStart(2,"0");
  document.getElementById("minutes").textContent = String(Math.floor(total % 3600 / 60)).padStart(2,"0");
  document.getElementById("seconds").textContent = String(total % 60).padStart(2,"0");
}
function unlockBirthday() {
  if (unlocked) return;
  unlocked = true;
  document.getElementById("birthdayLock").classList.add("hidden");
  document.getElementById("mainSite").classList.remove("hidden");
  document.title = "Happy Birthday Khusssss ♡";
  window.scrollTo(0,0);
  toast("Your birthday universe is open! ♡");
}
updateCountdown();
setInterval(updateCountdown,1000);

/* DAILY QUOTE: SAME QUOTE ALL DAY, NEW QUOTE AT MIDNIGHT IST */
const dailyQuotes = [
"Your future is built by the little things you do today.",
"You don't need to have everything figured out. Just take the next step.",
"One small improvement every day can create a beautiful future.",
"Believe in the person you are becoming.",
"Your dreams deserve effort, patience, and courage.",
"Don't compare your chapter one to someone else's chapter twenty.",
"Progress is progress, even when nobody notices.",
"A difficult day doesn't mean you have a difficult future.",
"Be patient with yourself. Growth takes time.",
"Your habits today are shaping your life tomorrow.",
"You are allowed to start again as many times as you need.",
"Choose progress over perfection.",
"Your future self will thank you for the effort you make today.",
"Keep learning. Keep growing. Keep believing.",
"Small steps can take you to extraordinary places.",
"You don't have to be the best today. Just be willing to improve.",
"Your potential is bigger than your current fears.",
"Turn your worries into plans and your plans into action.",
"A better future begins with one brave decision.",
"Rest when you need to, but don't give up on yourself.",
"Success is built quietly before it is celebrated publicly.",
"Let your goals be bigger than your excuses.",
"Be proud of how far you have come, even if you aren't there yet.",
"You can grow at your own pace and still achieve beautiful things.",
"Every mistake can teach you something valuable.",
"Your worth is not measured by your achievements.",
"Protect your peace while pursuing your dreams.",
"Be consistent, even when motivation is quiet.",
"The person you become matters as much as the things you achieve.",
"You are never too late to learn something new.",
"Give your dreams a chance before you give your doubts a voice.",
"Your life doesn't need to look like anyone else's to be meaningful.",
"Keep promises to yourself, especially the small ones.",
"Confidence grows when you keep showing up for yourself.",
"Let difficult moments make you wiser, not hopeless.",
"A slow journey can still lead to a wonderful destination.",
"Your future is not decided by one bad day.",
"Celebrate your progress without waiting for perfection.",
"You can be a work in progress and still be proud of yourself.",
"Make choices your future self will feel grateful for.",
"Discipline is choosing what matters over what feels easy.",
"Every new skill begins with being a beginner.",
"Don't fear change. Sometimes it leads you to yourself.",
"You deserve the same kindness you give to others.",
"Be brave enough to choose a path that feels right for you.",
"The best investment is often the effort you put into yourself.",
"A peaceful mind is part of a successful life.",
"Keep your heart kind and your boundaries strong.",
"You can do difficult things one step at a time.",
"Your dreams need action, not just imagination.",
"Celebrate the little wins. They are part of the bigger story.",
"You are capable of more than you discover by staying comfortable.",
"Don't let a temporary setback become a permanent belief.",
"Your future can be different from your past.",
"Make room for growth, even when it feels uncomfortable.",
"Be curious about life and patient with your progress.",
"You don't need everyone's approval to build a meaningful life.",
"A little courage today can open a new door tomorrow.",
"The way forward is often one small step at a time.",
"Keep going for the dreams that still make your heart hopeful.",
"Your kindness is a strength. Your ambition can be one, too.",
"Learn to begin before you feel completely ready.",
"Your timeline is your own. There is no need to rush your life.",
"Take care of your health while working toward your goals.",
"Don't forget to enjoy the life you are working so hard to build.",
"Be the person who encourages yourself to try again.",
"Growth begins when you become willing to learn.",
"A better tomorrow starts with the choices you make today.",
"Give yourself permission to outgrow old fears.",
"Your quiet efforts still count.",
"You can change direction without calling your journey a failure.",
"Let your curiosity take you somewhere new.",
"A setback is an event, not your identity.",
"Make your future a place you are excited to reach.",
"You don't need to hurry to become someone wonderful.",
"Be intentional with your time, energy, and dreams.",
"Sometimes the strongest move is to rest and begin again.",
"Trust yourself enough to take the first step.",
"Your progress doesn't need an audience to be real.",
"Choose friendships that help you feel respected and supported.",
"Every day gives you another chance to learn and improve.",
"Don't abandon a good dream just because it takes time.",
"Build a life that feels good from the inside, too.",
"Your confidence can grow through practice.",
"Let your goals guide you without forgetting your happiness.",
"You can be gentle with yourself and still aim high.",
"The effort you make today is part of tomorrow's possibilities.",
"Keep moving forward, even if your steps are small.",
"You deserve a future filled with purpose and peace.",
"You are allowed to dream beyond what you know today.",
"Let every new challenge teach you a new strength.",
"Your next chapter can begin with a simple decision.",
"Success means more when it aligns with your values.",
"Don't mistake a slow season for a wasted season.",
"Keep becoming someone you respect.",
"Your life can grow in beautiful directions you haven't imagined yet.",
"Be patient with the process and honest about the effort.",
"One day, today's effort may become the story that inspires you.",
"Keep your dreams alive, and give them practical steps to follow.",
"May you grow into a future that feels peaceful, meaningful, and truly yours."
];

function getIndiaDate() {
  const parts = new Intl.DateTimeFormat("en-CA", {
    timeZone:"Asia/Kolkata", year:"numeric", month:"2-digit", day:"2-digit"
  }).formatToParts(new Date());
  const get = type => parts.find(part => part.type === type).value;
  return `${get("year")}-${get("month")}-${get("day")}`;
}
function updateDailyQuote() {
  const quoteEl = document.getElementById("dailyQuote");
  const dateEl = document.getElementById("dailyQuoteDate");
  if (!quoteEl || !dateEl) return;

  const today = getIndiaDate();
  if (today > "2027-06-04") {
    quoteEl.textContent = "Your future is still unfolding. Keep learning, growing, and believing in yourself.";
    dateEl.textContent = "Your next chapter starts today ♡";
    return;
  }

  // The sequence begins on October 26, 2026, and advances once per Indian calendar day.
  const start = Date.UTC(2026,9,26);
  const currentParts = today.split("-").map(Number);
  const current = Date.UTC(currentParts[0],currentParts[1]-1,currentParts[2]);
  const dayIndex = Math.floor((current - start) / 86400000);
  const index = ((dayIndex % dailyQuotes.length) + dailyQuotes.length) % dailyQuotes.length;

  quoteEl.textContent = "“" + dailyQuotes[index] + "”";
  const readableDate = new Intl.DateTimeFormat("en-IN", {
    timeZone:"Asia/Kolkata", day:"numeric", month:"long", year:"numeric"
  }).format(new Date());
  dateEl.textContent = "Today's thought · " + readableDate;
}
updateDailyQuote();
// Recheck periodically, including if the page stays open across midnight.
setInterval(updateDailyQuote,60000);

/* MUSIC: WORKS BEFORE AND AFTER UNLOCKING */
async function toggleMusic() {
  const buttons = ["lockPlay","mainPlay"].map(id => document.getElementById(id));
  if (audio.paused) {
    try {
      await audio.play();
      buttons.forEach(button => { if (button) button.textContent = "❚❚ Pause Song"; });
      toast("Your song is playing ♡");
    } catch (error) {
      toast("Check that Song22.mp3 is uploaded beside index.html.");
    }
  } else {
    audio.pause();
    buttons.forEach(button => { if (button) button.textContent = "▶ Play Song"; });
  }
}
audio.addEventListener("play",() => ["lockPlay","mainPlay"].forEach(id => {
  const button = document.getElementById(id); if (button) button.textContent = "❚❚ Pause Song";
}));
audio.addEventListener("pause",() => ["lockPlay","mainPlay"].forEach(id => {
  const button = document.getElementById(id); if (button) button.textContent = "▶ Play Song";
}));

/* FLOATING HEARTS AND SPARKLES */
const layer = document.getElementById("particles");
const symbols = ["♡","✦","✧","⋆","♥","✩","·"];
function makeParticle() {
  if (document.hidden) return;
  const el = document.createElement("span");
  el.className = "particle";
  el.textContent = symbols[Math.floor(Math.random()*symbols.length)];
  el.style.left = Math.random()*100 + "%";
  el.style.fontSize = 10 + Math.random()*18 + "px";
  el.style.animationDuration = 7 + Math.random()*10 + "s";
  el.style.color = Math.random()>.5 ? "#ff9ed4" : "#d3b5ff";
  layer.appendChild(el);
  setTimeout(() => el.remove(),18000);
}
setInterval(makeParticle,450);

/* TOAST */
let toastTimer;
function toast(message) {
  const el = document.getElementById("toast");
  el.textContent = message; el.classList.add("show");
  clearTimeout(toastTimer);
  toastTimer = setTimeout(() => el.classList.remove("show"),2600);
}

/* 30 BIRTHDAY WISHES */
const wishes = [
"May happiness find you in the smallest moments.",
"May your dreams become plans, and your plans become beautiful memories.",
"May you always have the courage to begin again.",
"May you find people who appreciate your beautiful heart.",
"May laughter visit your home every day.",
"May your confidence grow stronger with every new chapter.",
"May you discover new places and collect unforgettable memories.",
"May your hard work bring you opportunities you once imagined.",
"May you never forget how much you are worth.",
"May peace find you on your busiest days.",
"May your future surprise you in the loveliest ways.",
"May you have the strength to leave behind what hurts you.",
"May you always feel safe being your true self.",
"May your smile return quickly after a difficult day.",
"May your goals feel closer with every step you take.",
"May you be surrounded by genuine love and loyalty.",
"May you find beauty in ordinary days.",
"May you always have a reason to be proud of yourself.",
"May every new beginning bring you hope.",
"May you keep your kindness without losing your boundaries.",
"May you laugh until your cheeks hurt.",
"May your health, peace, and happiness always matter.",
"May you be brave enough to follow your own path.",
"May your life be rich in love and meaningful moments.",
"May you feel appreciated even when nobody says it aloud.",
"May your worries become lighter and your hopes brighter.",
"May you always have a place where you feel at home.",
"May your future be filled with wonderful surprises.",
"May you continue to grow without losing your beautiful self.",
"May this year be one of your happiest chapters yet."
];
document.getElementById("wishGrid").innerHTML = wishes.map((w,i) =>
  `<article class="card"><span class="pill">Wish ${String(i+1).padStart(2,"0")}</span><p>${w}</p></article>`
).join("");

/* 100 SISTER QUOTES */
const quotes = [
"A sister is a little piece of home you can carry everywhere.",
"Life gave me many blessings, and having you as my sister is one of them.",
"A sister can make an ordinary day feel like a treasured memory.",
"Some bonds need no explanation; sisterhood is one of them.",
"A sister is a friend whose place in your story is forever special.",
"Distance can change where we stand, but it cannot erase the love we share.",
"A sister's happiness is a beautiful reason to smile.",
"Home is not always a place; sometimes it is the people we love.",
"A sister is part of your childhood and a blessing in your growing years.",
"One of life's sweetest gifts is someone you can call your sister.",
"A sister knows pieces of your story that the world may never hear.",
"The best sisterhood is built with love, patience, laughter, and care.",
"A sister makes family memories more colourful.",
"Having a sister means having another heart to celebrate life's little joys.",
"Some people make life brighter simply by being in it; you are one of them.",
"A sister is a forever chapter in the book of your life.",
"May our bond always be stronger than our misunderstandings.",
"Growing older is easier when the love of family grows with you.",
"A sister is a beautiful reminder that you never begin life alone.",
"No perfect words can measure the value of a loving sister.",
"A sister's smile can turn a difficult day into a softer one.",
"Love makes a family, and care keeps its memories alive.",
"Every sister has a special place no one else can fill.",
"A sister is not just someone beside you, but someone you carry in your heart.",
"May we always find a reason to laugh together.",
"Some memories fade in detail but remain warm in the heart.",
"A sister is a familiar voice in a world that keeps changing.",
"The little things we share often become the memories we treasure most.",
"Being sisters means having a bond that keeps finding new ways to grow.",
"A sister deserves kindness on her birthday and on every ordinary day.",
"Family is one of life's quietest and strongest blessings.",
"A sister is a friend made special by a shared story.",
"May your life always return the kindness you give to others.",
"A loving sister is a treasure that cannot be measured in money.",
"Your dreams matter, your voice matters, and your happiness matters.",
"A sister should never have to hide her tears to prove her strength.",
"May you always feel free to be your real, wonderful self.",
"Your worth is not decided by anyone else's opinion.",
"A sister's heart deserves the same care she gives to others.",
"May you always find courage when the road becomes uncertain.",
"Every new year of life is another chance to discover your strength.",
"A sister can be both a familiar memory and a fresh inspiration.",
"The best gifts are the people who make life meaningful.",
"May your laughter stay loud and your worries become lighter.",
"Even when we disagree, I hope our care for each other remains.",
"A sister is part of the story that made you who you are.",
"May we keep collecting moments worth remembering.",
"Your presence adds something beautiful to our family.",
"A sister's love is shown in little acts of care, not only big words.",
"May you be proud of how far you have come.",
"You deserve a life that feels peaceful as well as exciting.",
"May you never shrink yourself to fit someone else's expectations.",
"Your kindness is a strength, and your boundaries are important too.",
"A sister is a reminder that love can grow through every season.",
"May the future give you reasons to believe in yourself.",
"The world is brighter when you allow your own light to shine.",
"Your birthday celebrates not just another year, but the person you are becoming.",
"May your courage be bigger than your fear.",
"A sister deserves friendships that feel safe, honest, and joyful.",
"May you never forget to celebrate your own progress.",
"Small steps still take you toward beautiful places.",
"A sister's dreams deserve encouragement, not limits.",
"May life surprise you with the good you never saw coming.",
"Your happiness is worth protecting.",
"May you always know the difference between being needed and being valued.",
"A sister is someone whose story will always matter to you.",
"May you have the courage to choose what brings you peace.",
"Even the quietest moments can become treasured memories.",
"May your heart stay gentle and your spirit stay brave.",
"Your future does not need to look like anyone else's to be wonderful.",
"May you always find people who celebrate your success sincerely.",
"A sister is a lovely part of the story we call family.",
"May you keep learning, growing, laughing, and dreaming.",
"Never forget that rest is allowed and asking for help is brave.",
"May every difficult chapter teach you without defining you.",
"A sister's birthday is a perfect moment to celebrate her whole self.",
"May your days hold more genuine smiles than forced ones.",
"May you find beauty in the person you are today.",
"Your dreams are worth the patience it takes to reach them.",
"A sister can be a memory keeper, a cheerleader, and a lifelong blessing.",
"May you always have a reason to hope.",
"May the people around you make you feel appreciated and understood.",
"A sister's value does not depend on what she achieves.",
"May you give yourself the same kindness you offer others.",
"Every birthday is another page waiting for your own story.",
"May your life be full of honest love and meaningful moments.",
"May you never lose the little things that make you uniquely you.",
"A sister deserves to feel celebrated even when it is not her birthday.",
"May your heart find peace after every storm.",
"Your laughter is a little gift to the people who love you.",
"May you always have the freedom to grow into yourself.",
"A sister is part of your roots and part of your memories.",
"May your future be kinder than your fears predict.",
"May you be surrounded by people who respect your boundaries.",
"Some bonds become more meaningful with every year that passes.",
"May your dreams stay alive even when progress feels slow.",
"A sister is a blessing to appreciate, not a person to take for granted.",
"May your birthday begin a year filled with hope, health, and happiness.",
"No matter how much life changes, I hope you always know you are loved."
];
let quoteIndex = 0, visibleQuotes = 12;

function newQuote() {
  quoteIndex = (quoteIndex + 1 + Math.floor(Math.random()*9)) % quotes.length;
  document.getElementById("randomQuote").textContent = "“" + quotes[quoteIndex] + "”";
  document.getElementById("quoteAuthor").textContent = "For Khusssss ♡";
  document.getElementById("quoteCounter").textContent = `Quote ${quoteIndex+1} of ${quotes.length}`;
}
function copyText(text) {
  if (navigator.clipboard && navigator.clipboard.writeText) {
    navigator.clipboard.writeText(text).then(() => toast("Copied ♡")).catch(() => toast(text));
  } else toast(text);
}
function copyQuote() { copyText(document.getElementById("randomQuote").textContent); }
function copySpecificQuote(i) { copyText("“" + quotes[i] + "”"); }

function renderQuotes(filter="") {
  const matches = quotes.map((q,i)=>({q,i})).filter(x=>x.q.toLowerCase().includes(filter.toLowerCase()));
  document.getElementById("quoteGrid").innerHTML = matches.slice(0,visibleQuotes).map(x =>
    `<article class="card"><span class="pill">Sister Quote ${x.i+1}</span><p>“${x.q}”</p><button class="secondary" onclick="copySpecificQuote(${x.i})">Copy Quote</button></article>`
  ).join("");
  document.getElementById("moreQuotes").style.display = matches.length>visibleQuotes ? "inline-block" : "none";
  if (!matches.length) document.getElementById("quoteGrid").innerHTML = '<p>No quotes found. Try another word.</p>';
}
function showMoreQuotes() { visibleQuotes += 12; renderQuotes(document.getElementById("quoteSearch").value); }
document.getElementById("quoteSearch").addEventListener("input",e=>{visibleQuotes=12;renderQuotes(e.target.value);});
renderQuotes();

/* PHOTO GALLERY */
const galleryItems = [
["K1.jpg","A memory to keep"],["K2.jpg","A little piece of happiness"],
["K3.jpg","One for the memories"],["K4.jpg","A moment worth saving"],
["K5.jpg","Beautiful little things"],["K6.jpg","Our story in pictures"],
["K7.jpg","A memory close to my heart"],["K8.jpg","Another lovely chapter"],
["K9.jpg","Moments that matter"],["K10.jpg","A smile worth remembering"],
["K12.jpg","A little reminder of love"]
];
document.getElementById("gallery").innerHTML = galleryItems.map(([src,caption])=>`
  <article class="card memory-card">
    <img class="photo" src="${src}" alt="${caption}" loading="lazy"
    onerror="this.style.display='none';this.nextElementSibling.style.display='grid'">
    <div class="photo" style="display:none;place-items:center;color:#ffb7e0">Add ${src} to your repository</div>
    <p>${caption}</p>
  </article>
`).join("") + `
  <article class="card memory-card">
    <video class="photo" controls preload="metadata" playsinline>
      <source src="K11.mp4" type="video/mp4">Your browser does not support this video.
    </video><p>A moving memory, kept forever.</p>
  </article>`;

/* 100 REASONS */
const reasons = [
"Your place in the family is unique.","You deserve to be celebrated.","Your dreams are worth taking seriously.",
"You bring your own personality to every room.","You are allowed to grow and change.","Your feelings deserve to be heard.",
"You deserve peaceful days.","You deserve genuine friendships.","You can learn from mistakes without being defined by them.",
"You have a story that belongs to you.","Your laughter can make moments memorable.","You deserve to feel safe and respected.",
"You do not have to be perfect.","You can be proud of small progress.","You deserve to be treated with kindness.",
"You can take your time finding your path.","Your ideas are worth sharing.","You deserve opportunities to grow.",
"You can ask for help when you need it.","You have the right to say no.","You deserve love that feels honest.",
"You can begin again after a hard day.","Your future is full of possibilities.","You deserve time to rest.",
"You can choose what matters to you.","You are allowed to celebrate yourself.","You deserve people who listen.",
"You can be brave and still feel afraid.","You can change your mind as you learn.","You deserve to be appreciated.",
"Your happiness matters.","You can build a life that feels right for you.","You deserve respect in every relationship.",
"You can learn new things at any age.","You deserve to feel proud of your progress.","You do not need to compare your journey.",
"You can protect your peace.","You deserve laughter and fun.","You can make mistakes and keep growing.",
"You deserve to be understood.","You can follow your curiosity.","You deserve to feel included.",
"You can set healthy boundaries.","You deserve encouragement.","You can make meaningful memories.",
"You have your own strengths.","You can choose hope during uncertainty.","You deserve kindness from yourself, too.",
"You can keep your individuality.","You deserve a future you look forward to.","You are part of our family's story.",
"You can take one step at a time.","You deserve to feel seen.","You can stand up for what matters.",
"You deserve to learn without shame.","You can find joy in simple things.","You deserve care on difficult days.",
"You can have goals that change over time.","You deserve relationships with mutual respect.","You can be proud of your resilience.",
"You deserve room to express yourself.","You can learn from the past.","You deserve to be listened to patiently.",
"You can make your own decisions.","You deserve moments of calm.","You can keep discovering your talents.",
"You deserve people who cheer for you.","You can take breaks without guilt.","You deserve to feel hopeful.",
"You can make your own definition of success.","You deserve to be treated fairly.","You can ask for support.",
"You deserve to feel comfortable being yourself.","You can celebrate another person's success, too.","You deserve honesty.",
"You can turn experience into wisdom.","You deserve joy that does not depend on perfection.","You can be gentle with yourself.",
"You deserve to have your boundaries respected.","You can keep learning about who you are.","You deserve a chance to try.",
"You can create traditions of your own.","You deserve to feel appreciated for who you are.","You can take a different route.",
"You deserve support for your goals.","You can choose what you want to carry forward.","You deserve love without pretending.",
"You can find beauty in ordinary moments.","You deserve time to think.","You can make new memories.",
"You deserve a birthday full of warmth.","You can keep your sense of wonder.","You deserve to celebrate your growth.",
"You can ask questions and stay curious.","You deserve a life with room for joy.","You can face change one day at a time.",
"You deserve to be surrounded by care.","You are worth celebrating today and every day."
];
document.getElementById("reasonGrid").innerHTML = reasons.map((r,i)=>
  `<div class="reason"><b>${String(i+1).padStart(2,"0")}.</b>${r}</div>`
).join("");

/* HIDDEN MESSAGES AND SURPRISES */
const secrets = [
"Even when I don't say it often, I'm glad you're my sister. ♡",
"Your happiness matters to me more than a perfect birthday website ever could.",
"May you always find people who see the wonderful person you are.",
"Whenever life feels heavy, remember that you deserve support and care.",
"Here's a little reminder: you are loved on ordinary days, too.",
"I hope your next chapter brings you closer to the life you dream about.",
"You don't have to do everything alone. It's okay to lean on family.",
"May your heart always have reasons to hope.",
"You deserve good things simply because you are you.",
"Happy Birthday, Khusssss. This little corner of the internet is yours."
];
let secretIndex=0;
function revealSecret() {
  document.getElementById("secretMessage").textContent=secrets[secretIndex];
  secretIndex=(secretIndex+1)%secrets.length; toast("A little message, just for you ♡");
}
const hugs=[
"Sending you the biggest virtual hug. Imagine it lasting as long as you need. ♡",
"One hug for your smile, one for your dreams, and one for every difficult day.",
"Pause for a second. Breathe in. You deserve kindness and a little comfort.",
"Consider this your reminder that you are appreciated and loved.",
"Wrapping this little message around you like a warm, comforting hug."
];
let hugIndex=0;
function virtualHug() {
  document.getElementById("hugMessage").textContent=hugs[hugIndex];
  hugIndex=(hugIndex+1)%hugs.length; celebrate(false);
}
const fortunes=[
"Something wonderful can begin with one small brave step.",
"Be patient with yourself; growth is not always loud.",
"A new memory is waiting somewhere in your next chapter.",
"Your kindness can matter more than you realise.",
"Give your dreams time and give yourself credit for trying.",
"A peaceful heart is a beautiful kind of success.",
"May the next year bring you a reason to smile unexpectedly.",
"Keep your eyes open for small joys; they often become big memories.",
"You are allowed to start again as many times as you need.",
"Your story is still unfolding. There are good pages ahead."
];
function fortune() { document.getElementById("fortuneMessage").textContent=fortunes[Math.floor(Math.random()*fortunes.length)]; }

let flowerCount=0;
const flowers=["🌸","🌷","🌼","✿","💐","🌺","❀","🌻"];
function plantFlower() {
  if (flowerCount===0) document.getElementById("garden").innerHTML="";
  flowerCount++;
  const el=document.createElement("span");
  el.textContent=flowers[Math.floor(Math.random()*flowers.length)];
  el.title="A wish for Khusssss";
  document.getElementById("garden").appendChild(el);
  document.getElementById("flowerCount").textContent="Flowers planted: "+flowerCount;
  toast("A new flower for your happiness ♡");
}
function celebrate(showToast=true) {
  for(let i=0;i<24;i++) setTimeout(makeParticle,i*45);
  if(showToast) toast("Sending birthday love to Khusssss! ♡");
}
</script>
</body>
</html>
