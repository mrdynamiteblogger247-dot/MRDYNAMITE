
<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#080808">
<meta name="description" content="MRDYNAMITE - Official Personal Brand">
<title>👑 MRDYNAMITE | Official</title>

<style>
@import url('https://fonts.googleapis.com/css2?family=Vazirmatn:wght@400;500;700;800;900&display=swap');

:root{
  --gold:#e8b85d;
  --gold2:#ffe4a3;
  --dark:#080808;
  --card:#121212;
  --line:#3b2b18;
  --text:#fff8eb;
  --muted:#b5a894;
}

*{box-sizing:border-box;margin:0;padding:0}

html{scroll-behavior:smooth}

body{
  background:#030303;
  color:var(--text);
  font-family:'Vazirmatn',Tahoma,Arial,sans-serif;
  overflow-x:hidden;
}

button,a{font:inherit}
button,a{ -webkit-tap-highlight-color:transparent }

button:focus-visible,a:focus-visible{
  outline:2px solid var(--gold2);
  outline-offset:4px;
}

.page{
  position:relative;
  max-width:560px;
  margin:auto;
  min-height:100vh;
  overflow:hidden;
  background:
    radial-gradient(ellipse at 50% -10%,#4a210e 0%,#160c07 28%,#080808 60%);
}

/* افکت ذرات نور */
#particles{
  position:absolute;
  inset:0;
  width:100%;
  height:100%;
  pointer-events:none;
  opacity:.65;
}

/* نوار بالا */
.nav{
  position:relative;
  z-index:2;
  display:flex;
  align-items:center;
  justify-content:space-between;
  padding:22px 20px;
  border-bottom:1px solid #2b2116;
}

.nav-logo{
  font-size:17px;
  font-weight:900;
  letter-spacing:1px;
  color:var(--gold);
}

.nav-tag{
  font-size:10px;
  color:#a99a82;
  letter-spacing:1px;
}

/* بخش اصلی */
.hero{
  position:relative;
  z-index:1;
  text-align:center;
  padding:36px 20px 42px;
}

.crown{
  font-size:54px;
  filter:drop-shadow(0 0 20px #e8b85d88);
  animation:float 4s ease-in-out infinite;
}

@keyframes float{
  0%,100%{transform:translateY(0)}
  50%{transform:translateY(-8px)}
}

.logo{
  margin-top:8px;
  font-size:clamp(30px,8.5vw,49px);
  line-height:1.3;
  font-weight:900;
  letter-spacing:2px;
  color:var(--gold2);
  text-shadow:
    0 0 8px #e8b85d88,
    0 0 30px #9c551e66;
}

.official{
  margin-top:12px;
  font-size:10px;
  letter-spacing:4px;
  color:#a99a82;
}

.badge{
  display:inline-block;
  margin:24px 0 18px;
  padding:8px 15px;
  border:1px solid #735127;
  border-radius:50px;
  color:var(--gold);
  background:#211508aa;
  font-size:11px;
  box-shadow:0 0 20px #9c551e22;
}

.hero h1{
  font-size:clamp(24px,6.5vw,34px);
  line-height:1.8;
  font-weight:900;
}

.hero h1 span{color:var(--gold)}

.hero p{
  max-width:410px;
  margin:12px auto 0;
  color:var(--muted);
  font-size:13px;
  line-height:2.1;
}

/* عکس جایگزین */
.photo{
  position:relative;
  width:190px;
  height:190px;
  margin:28px auto 24px;
  border-radius:50%;
  padding:4px;
  background:linear-gradient(135deg,#fff0b0,#9b621f,#e8b85d,#5c3516);
  box-shadow:
    0 0 0 5px #1d140b,
    0 0 35px #c68c3d55;
}

.photo-inner{
  width:100%;
  height:100%;
  border-radius:50%;
  overflow:hidden;
  background:
    radial-gradient(circle at 50% 25%,#6e4b23,#25170b 45%,#090909);
  display:flex;
  align-items:center;
  justify-content:center;
  flex-direction:column;
}

.photo-inner .emoji{
  font-size:62px;
  filter:drop-shadow(0 0 12px #e8b85d66);
}

.photo-inner small{
  color:#d5ae69;
  font-size:10px;
  margin-top:7px;
  letter-spacing:1px;
}

/* دکمه‌ها */
.btn{
  display:flex;
  justify-content:center;
  align-items:center;
  gap:10px;
  width:100%;
  min-height:54px;
  padding:15px 18px;
  border-radius:13px;
  font-size:14px;
  font-weight:800;
  text-decoration:none;
  cursor:pointer;
  transition:transform .2s,box-shadow .2s;
}

.btn:active{transform:scale(.97)}

.gold-btn{
  color:#1b1105;
  background:linear-gradient(105deg,#a66b20,#ffe4a3,#d5a34e);
  box-shadow:0 8px 28px #b47b3033;
}

.gold-btn:hover{box-shadow:0 8px 35px #d5a34e66}

.dark-btn{
  color:var(--gold2);
  background:#17110b;
  border:1px solid #604523;
  margin-top:12px;
}

.hero-buttons{
  max-width:400px;
  margin:25px auto 0;
}

/* کارت آمار */
.stats{
  position:relative;
  z-index:1;
  display:grid;
  grid-template-columns:repeat(3,1fr);
  gap:9px;
  padding:0 20px;
}

.stat{
  text-align:center;
  padding:18px 5px;
  background:#15110d;
  border:1px solid var(--line);
  border-radius:14px;
}

.stat strong{
  display:block;
  font-size:25px;
  color:var(--gold);
  margin-bottom:5px;
}

.stat span{
  color:#a99b87;
  font-size:11px;
}

/* بخش معرفی */
.section{
  position:relative;
  z-index:1;
  padding:38px 20px;
}

.section-title{
  text-align:center;
  font-size:22px;
  font-weight:900;
  margin-bottom:12px;
}

.section-title span{color:var(--gold)}

.section-desc{
  text-align:center;
  color:var(--muted);
  font-size:13px;
  line-height:2.2;
}

.features{
  display:grid;
  grid-template-columns:repeat(2,1fr);
  gap:11px;
  margin-top:23px;
}

.feature{
  padding:19px 14px;
  background:linear-gradient(145deg,#17120c,#0e0e0e);
  border:1px solid #302316;
  border-radius:15px;
}

.feature-icon{font-size:27px;margin-bottom:10px}

.feature h3{
  font-size:14px;
  color:#f2d49b;
  margin-bottom:7px;
}

.feature p{
  font-size:11px;
  line-height:1.9;
  color:#a99d8c;
}

/* دعوت به فالو */
.follow-card{
  position:relative;
  overflow:hidden;
  text-align:center;
  padding:31px 20px;
  border:1px solid #6b4b22;
  border-radius:20px;
  background:
    radial-gradient(ellipse at 50% 0%,#3b210e,#171008 55%,#0e0e0e);
  box-shadow:0 0 40px #b0782b12;
}

.follow-card:before{
  content:'';
  position:absolute;
  top:-100px;
  left:50%;
  transform:translateX(-50%);
  width:230px;
  height:230px;
  border-radius:50%;
  border:1px solid #c08a3b22;
  box-shadow:0 0 0 30px #c08a3b0b,0 0 0 60px #c08a3b07;
}

.follow-card>*{position:relative}

.follow-card h2{
  font-size:23px;
  line-height:1.7;
}

.follow-card p{
  font-size:13px;
  color:#bdb09d;
  margin:10px 0 18px;
  line-height:2;
}

.handle{
  display:inline-block;
  direction:ltr;
  color:var(--gold2);
  font-size:19px;
  font-weight:900;
  letter-spacing:1px;
  margin-bottom:20px;
}

/* فوتر */
.footer{
  position:relative;
  z-index:1;
  padding:25px 20px;
  text-align:center;
  border-top:1px solid #2a2118;
  color:#766b5b;
  font-size:11px;
  line-height:2;
}

.footer strong{color:#b08b4d}

/* جداکننده */
.divider{
  height:1px;
  background:linear-gradient(90deg,transparent,#5a4020,transparent);
  margin:30px 0;
}

/* واکنش‌گرا */
@media(max-width:380px){
  .hero{padding:28px 15px 35px}
  .stats{padding:0 15px}
  .section{padding:32px 15px}
  .photo{width:165px;height:165px}
  .features{gap:8px}
}

@media(prefers-reduced-motion:reduce){
  *,*:before,*:after{
    animation-duration:.01ms!important;
    animation-iteration-count:1!important;
    scroll-behavior:auto!important;
  }
}
</style>
</head>

<body>

<div class="page" id="top">

<canvas id="particles" aria-hidden="true"></canvas>

<!-- نوار بالا -->
<nav class="nav">
  <div class="nav-logo">👑 MRDYNAMITE</div>
  <div class="nav-tag">OFFICIAL PAGE</div>
</nav>

<!-- هیرو -->
<section class="hero">

  <div class="crown">👑</div>

  <div class="logo">MRDYNAMITE</div>

  <div class="official">PERSONAL BRAND • 2026</div>

  <div class="badge">🔥 WELCOME TO MY WORLD 🔥</div>

  <h1>
    خاص بودن،<br>
    <span>یک انتخابه.</span>
  </h1>

  <p>
    به دنیای MRDYNAMITE خوش اومدی؛
    جایی برای استایل خاص، انرژی متفاوت
    و لحظه‌های ماندگار.
  </p>

  <!-- عکس جایگزین -->
  <div class="photo" aria-label="تصویر جایگزین MRDYNAMITE">
    <div class="photo-inner">
      <div class="emoji">👑</div>
      <small>MRDYNAMITE</small>
    </div>
  </div>

  <div class="hero-buttons">

    <a class="btn gold-btn"
       href="https://www.instagram.com/mr.dynamite247/"
       target="_blank"
       rel="noopener noreferrer">
      📸 فالو کن در اینستاگرام ↗
    </a>

    <a class="btn dark-btn" href="#about">
      ✨ درباره MRDYNAMITE
    </a>

  </div>

</section>

<!-- آمار -->
<section class="stats" aria-label="ویژگی‌های برند">
  <div class="stat">
    <strong>👑</strong>
    <span>استایل خاص</span>
  </div>
  <div class="stat">
    <strong>🔥</strong>
    <span>انرژی متفاوت</span>
  </div>
  <div class="stat">
    <strong>🎬</strong>
    <span>خاطرات ماندگار</span>
  </div>
</section>

<!-- معرفی -->
<section class="section" id="about">

  <h2 class="section-title">
    دنیای <span>MRDYNAMITE</span>
  </h2>

  <p class="section-desc">
    هر قاب یک داستانه، هر قدم یک امضا.
    همراه ما باش تا لحظه‌های خاص رو با هم بسازیم.
  </p>

  <div class="features">

    <div class="feature">
      <div class="feature-icon">🕶️</div>
      <h3>Luxury Style</h3>
      <p>استایل، جذابیت و ظاهر متفاوت در هر قاب.</p>
    </div>

    <div class="feature">
      <div class="feature-icon">🌍</div>
      <h3>Travel & Life</h3>
      <p>سفرها، رفاقت‌ها و خاطرات فراموش‌نشدنی.</p>
    </div>

    <div class="feature">
      <div class="feature-icon">🎥</div>
      <h3>Creative Reels</h3>
      <p>محتوای خلاقانه و لحظه‌های جذاب برای مخاطب.</p>
    </div>

    <div class="feature">
      <div class="feature-icon">🤝</div>
      <h3>Good Vibes</h3>
      <p>انرژی مثبت، رفاقت و همراهی با دوستان.</p>
    </div>

  </div>

  <div class="divider"></div>

  <!-- دعوت نهایی -->
  <div class="follow-card">

    <div style="font-size:40px;margin-bottom:10px">👑</div>

    <h2>عضو خانواده MRDYNAMITE شو!</h2>

    <p>
      اگه استایل خاص و انرژی خوب رو دوست داری،
      همین الان همراه ما باش.
    </p>

    <div class="handle">@mr.dynamite247</div>

    <a class="btn gold-btn"
       href="https://www.instagram.com/mr_dynamite247/"
       target="_blank"
       rel="noopener noreferrer">
      ❤️ همین الان فالو کن
    </a>

    <button class="btn dark-btn" id="shareBtn" type="button">
      📤 اشتراک‌گذاری صفحه
    </button>

    <p id="shareStatus" style="font-size:11px;margin-top:10px" aria-live="polite"></p>

  </div>

</section>

<footer class="footer">
  <strong>👑 MRDYNAMITE</strong><br>
  Official Personal Brand • All Rights Reserved
</footer>

</div>

<script>
/* افکت ذرات نور */
(function(){
  const canvas=document.getElementById('particles');
  const ctx=canvas.getContext('2d');
  if(!ctx)return;

  let width=0,height=0;
  let dots=[];
  let raf=0;
  const reduce=window.matchMedia &&
    window.matchMedia('(prefers-reduced-motion: reduce)').matches;

  function resize(){
    const dpr=Math.min(window.devicePixelRatio||1,2);
    width=canvas.clientWidth;
    height=canvas.clientHeight;
    canvas.width=Math.round(width*dpr);
    canvas.height=Math.round(height*dpr);
    ctx.setTransform(dpr,0,0,dpr,0,0);

    dots=Array.from({length:35},()=>({
      x:Math.random()*width,
      y:Math.random()*Math.max(height,600),
      r:Math.random()*1.5+.3,
      speed:Math.random()*.25+.08,
      alpha:Math.random()*.45+.15
    }));
  }

  function draw(){
    ctx.clearRect(0,0,width,height);

    for(const d of dots){
      ctx.beginPath();
      ctx.arc(d.x,d.y,d.r,0,Math.PI*2);
      ctx.fillStyle='rgba(232,184,93,'+d.alpha+')';
      ctx.fill();

      if(!reduce){
        d.y-=d.speed;
        if(d.y<-5){
          d.y=height+5;
          d.x=Math.random()*width;
        }
      }
    }

    if(!reduce)raf=requestAnimationFrame(draw);
  }

  resize();
  draw();

  window.addEventListener('resize',resize,{passive:true});

  if(reduce)cancelAnimationFrame(raf);
})();

/* اشتراک‌گذاری */
(function(){
  const btn=document.getElementById('shareBtn');
  const status=document.getElementById('shareStatus');

  btn.addEventListener('click',async function(){
    const data={
      title:'MRDYNAMITE 👑',
      text:'به صفحه رسمی MRDYNAMITE سر بزن!',
      url:window.location.href
    };

    if(navigator.share){
      try{
        await navigator.share(data);
        status.textContent='صفحه برای اشتراک‌گذاری آماده شد.';
      }catch(error){
        if(error.name!=='AbortError'){
          status.textContent='اشتراک‌گذاری انجام نشد.';
        }
      }
    }else{
      status.textContent='آدرس همین صفحه را از نوار مرورگر کپی کن و برای دوستانت بفرست.';
    }
  });
})();
</script>

</body>
</html>
