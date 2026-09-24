<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>NEURA STUDIO — صانع محتوى الذكاء الاصطناعي</title>
<meta name="description" content="فيديوهات ذكاء اصطناعي احترافية بأكثر من 6 دقائق">
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Cairo:wght@400;600&family=Tajawal:wght@700;800&family=Space+Grotesk:wght@500;700&display=swap">
<style>
/* ===== المتغيرات ===== */
:root{--bg:#0A0A0F;--bg2:#111827;--tx:#fff;--mut:#94A3B8;--v:#8B5CF6;--c:#06B6D4;--g:#F59E0B;--glass:rgba(255,255,255,.05);--bd:rgba(255,255,255,.1);--grad:linear-gradient(135deg,var(--v),var(--c));
box-sizing:border-box;padding-top:env(safe-area-inset-top,0px);padding-bottom:env(safe-area-inset-bottom,0px)}
:root[data-theme=light]{--bg:#F6F7FB;--bg2:#fff;--tx:#0F172A;--mut:#475569;--glass:rgba(255,255,255,.7);--bd:rgba(15,23,42,.1)}
@media(prefers-color-scheme:light){:root:not([data-theme=dark]):not([data-theme=light]){--bg:#0A0A0F}}
*{box-sizing:border-box;margin:0}
html{scroll-behavior:smooth;scroll-padding-top:calc(80px + env(safe-area-inset-top,0px))}
body{background:var(--bg);color:var(--tx);font:400 16px/1.7 Cairo,sans-serif;overflow-x:hidden;transition:background .4s,color .4s}
h1,h2,h3{font-family:Tajawal,sans-serif;font-weight:800;line-height:1.2}
a{color:inherit;text-decoration:none}
:focus-visible{outline:2px solid var(--g);outline-offset:3px}
.wrap{max-width:1100px;margin:auto;padding:0 20px}
section{padding:72px 0}
h2{font-size:clamp(26px,5vw,38px);margin-bottom:28px}
/* ===== الأزرار ===== */
.btn{display:inline-flex;align-items:center;gap:8px;border:0;border-radius:999px;padding:12px 26px;font:600 15px Cairo;color:#fff;background:var(--grad);cursor:pointer;position:relative;overflow:hidden;transition:transform .2s,box-shadow .2s;box-shadow:0 0 24px rgba(139,92,246,.35)}
.btn:hover{transform:translateY(-2px);box-shadow:0 0 34px rgba(6,182,212,.5)}
.btn.gold{background:var(--g);color:#1a1200;box-shadow:0 0 24px rgba(245,158,11,.5)}
.btn.ghost{background:var(--glass);border:1px solid var(--bd);color:var(--tx);box-shadow:none}
.rip{position:absolute;border-radius:50%;background:rgba(255,255,255,.4);transform:scale(0);animation:rp .6s linear;pointer-events:none}
@keyframes rp{to{transform:scale(4);opacity:0}}
/* ===== الشريط العلوي ===== */
nav{position:fixed;inset:0 0 auto 0;z-index:50;padding-top:env(safe-area-inset-top,0px);transition:.3s}
nav.s{background:var(--glass);backdrop-filter:blur(16px);border-bottom:1px solid var(--bd)}
nav .wrap{display:flex;align-items:center;gap:16px;height:68px}
.logo{display:flex;align-items:center;gap:8px;font:700 18px 'Space Grotesk';letter-spacing:.5px}
.logo small{font-weight:500;opacity:.7}
.links{display:flex;gap:22px;margin-inline-start:auto;color:var(--mut);font-size:14px}
.links a:hover{color:var(--tx)}
.ic{width:40px;height:40px;border-radius:50%;border:1px solid var(--bd);background:var(--glass);color:var(--tx);cursor:pointer;display:grid;place-items:center}
@media(max-width:860px){.links{display:none}nav .btn{margin-inline-start:auto}}
/* ===== الواجهة الرئيسية ===== */
.hero{min-height:100svh;display:grid;place-items:center;text-align:center;position:relative;padding:110px 0 60px;background:radial-gradient(60% 50% at 20% 20%,rgba(139,92,246,.28),transparent),radial-gradient(50% 45% at 85% 70%,rgba(6,182,212,.22),transparent)}
#pc{position:absolute;inset:0;width:100%;height:100%}
.hero .wrap{position:relative}
.av{width:150px;height:150px;border-radius:50%;padding:4px;margin:0 auto 24px;background:conic-gradient(var(--v),var(--c),var(--g),var(--v));animation:sp 6s linear infinite}
.av>div{width:100%;height:100%;border-radius:50%;background:var(--bg2);animation:sp 6s linear infinite reverse;overflow:hidden}
.av img,.av svg{width:100%;height:100%;object-fit:cover}
@keyframes sp{to{transform:rotate(360deg)}}
.hero h1{font:700 clamp(38px,9vw,84px)/1.05 'Space Grotesk';background:var(--grad);-webkit-background-clip:text;background-clip:text;color:transparent}
.role{font:800 clamp(20px,4vw,28px) Tajawal;margin:14px 0 8px;min-height:1.4em}
.hero p{color:var(--mut);max-width:520px;margin:0 auto 28px}
.cta{display:flex;gap:12px;justify-content:center;flex-wrap:wrap}
.empty{margin-top:16px;font-size:14px;color:var(--g)}
/* ===== الإحصائيات ===== */
.stats{display:grid;grid-template-columns:repeat(3,1fr);gap:14px}
.card{background:var(--glass);border:1px solid var(--bd);border-radius:20px;backdrop-filter:blur(12px);transition:.3s}
.card:hover{border-color:var(--v);box-shadow:0 0 30px rgba(139,92,246,.25)}
.stat{padding:26px 10px;text-align:center}
.stat b{display:block;font:700 clamp(28px,6vw,46px) 'Space Grotesk'}
.stat span{color:var(--mut);font-size:14px}
/* ===== الشبكات ===== */
.grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(280px,1fr));gap:18px}
.vid{overflow:hidden}
.th{aspect-ratio:16/9;background:var(--grad);display:grid;place-items:center;position:relative;opacity:.9}
.th i{position:absolute;bottom:8px;inset-inline-end:8px;background:rgba(0,0,0,.7);color:#fff;font:600 12px 'Space Grotesk';padding:2px 8px;border-radius:6px;font-style:normal}
.vid h3{font-size:17px;padding:14px 16px 4px}.vid p{padding:0 16px 16px;color:var(--mut);font-size:13px}
.feat{padding:26px}.feat svg{width:34px;height:34px;stroke:var(--c);fill:none;stroke-width:1.6;margin-bottom:12px}
.feat h3{font-size:19px;margin-bottom:6px}.feat p{color:var(--mut);font-size:14px}
footer{border-top:1px solid var(--bd);padding:36px 0;text-align:center;color:var(--mut);font-size:14px}
footer nav{position:static}
/* ===== النافذة والإشعار ===== */
.ov{position:fixed;inset:0;z-index:90;background:rgba(0,0,0,.65);backdrop-filter:blur(6px);display:none;place-items:center;padding:20px}
.ov.on{display:grid}
.md{width:100%;max-width:440px;background:var(--bg2);border:1px solid var(--bd);border-radius:24px;padding:28px;animation:pop .3s}
@keyframes pop{from{transform:scale(.92);opacity:0}}
.md h3{font-size:24px;margin-bottom:14px}
.md input{width:100%;padding:13px 16px;border-radius:14px;border:1px solid var(--bd);background:var(--bg);color:var(--tx);font:400 15px Cairo;direction:ltr;text-align:left}
.md input.bad{border-color:#EF4444}
.err{color:#EF4444;font-size:13px;min-height:22px;margin-top:6px}
.md small{display:block;color:var(--mut);margin:6px 0 18px;font-size:13px}
.row{display:flex;gap:10px}
#toast{position:fixed;bottom:calc(24px + env(safe-area-inset-bottom,0px));left:50%;transform:translate(-50%,120px);z-index:99;background:var(--bg2);border:1px solid #10B981;border-radius:14px;padding:12px 22px;transition:.4s}
#toast.on{transform:translate(-50%,0)}
#ld{position:fixed;inset:0;z-index:200;background:var(--bg);display:grid;place-items:center;transition:opacity .6s}
#ld.off{opacity:0;pointer-events:none}
#ld svg{width:90px;animation:pl 1.2s infinite alternate}
@keyframes pl{to{transform:scale(1.15);filter:drop-shadow(0 0 16px var(--v))}}
@media(prefers-reduced-motion:reduce){*{animation:none!important;transition:none!important}}
</style>
</head>
<body>
<!-- شاشة التحميل -->
<div id="ld"><svg viewBox="0 0 48 48"><use href="#lg"/></svg></div>
<svg width="0" height="0" style="position:absolute"><defs>
<linearGradient id="gr" x1="0" y1="0" x2="1" y2="1"><stop offset="0" stop-color="#8B5CF6"/><stop offset="1" stop-color="#06B6D4"/></linearGradient>
<!-- الشعار: شبكة عصبية -->
<g id="lg" fill="none" stroke="url(#gr)" stroke-width="2.4" stroke-linecap="round"><circle cx="24" cy="10" r="4"/><circle cx="9" cy="30" r="4"/><circle cx="39" cy="30" r="4"/><circle cx="24" cy="40" r="3"/><path d="M22 14 11 27M26 14l11 13M13 31l8 8M35 31l-8 8M13 30h22"/></g></defs></svg>

<nav id="nav"><div class="wrap">
 <a class="logo" href="#top" aria-label="NEURA STUDIO"><svg width="34" height="34" viewBox="0 0 48 48" style="filter:drop-shadow(0 0 6px #8B5CF6)"><use href="#lg"/></svg>NEURA <small>STUDIO</small></a>
 <div class="links"><a href="#top">الرئيسية</a><a href="#videos">أحدث الفيديوهات</a><a href="#tools">الأدوات</a></div>
 <button class="btn gold" id="lk" data-open="modal">⭐ ربط القناة</button>
 <button class="ic" id="th" aria-label="تبديل الوضع">◐</button>
</div></nav>

<header class="hero" id="top">
 <canvas id="pc" aria-hidden="true"></canvas>
 <div class="wrap">
  <!-- data-avatar: ضع رابط صورتك الحقيقية هنا لاحقاً -->
  <div class="av" data-avatar=""><div><svg viewBox="0 0 100 100"><rect width="100" height="100" fill="#111827"/><circle cx="50" cy="38" r="17" fill="url(#gr)"/><path d="M16 96c4-26 20-34 34-34s30 8 34 34z" fill="url(#gr)"/></svg></div></div>
  <h1>Mohamed Ben Hanoun</h1>
  <div class="role" id="ty"></div>
  <p>أصنع فيديوهات ذكاء اصطناعي احترافية بأكثر من 6 دقائق</p>
  <div class="cta"><a class="btn gold" id="hb" href="#" data-open="modal">ربط القناة</a><a class="btn ghost" href="#videos">استكشف الموقع</a></div>
  <div class="empty" id="em">لم يتم ربط القناة بعد</div>
 </div>
</header>

<section style="padding-top:0"><div class="wrap stats">
 <div class="card stat"><b data-n="0">0</b><span>المشتركون</span></div>
 <div class="card stat"><b data-n="0">0</b><span>الفيديوهات</span></div>
 <div class="card stat"><b data-n="0">0</b><span>المشاهدات</span></div>
</div></section>

<section id="videos"><div class="wrap"><h2>أحدث الفيديوهات</h2><div class="grid" id="vg"></div></div></section>

<section id="tools"><div class="wrap"><h2>أدوات الاستوديو</h2><div class="grid" data-api-slot="tools">
 <div class="card feat"><svg viewBox="0 0 24 24"><rect x="3" y="5" width="18" height="14" rx="3"/><path d="m10 9 5 3-5 3z"/></svg><h3>إنشاء فيديو</h3><p>حوّل نصاً أو صوتاً أو صورة إلى فيديو بمقاسات ومدد مختلفة.</p></div>
 <div class="card feat"><svg viewBox="0 0 24 24"><path d="M4 5h16v11H9l-5 4z"/></svg><h3>الدردشة الذكية</h3><p>مساعد يعرف قناتك ويقترح أفكاراً وسكريبتات وكلمات مفتاحية.</p></div>
 <div class="card feat"><svg viewBox="0 0 24 24"><path d="M12 3v12M8 8v4M16 6v8M4 10v2M20 9v4M12 19v2"/></svg><h3>تحويل النص لصوت</h3><p>50 صوتاً بعشر لغات، مع التحكم في السرعة والنبرة.</p></div>
 <div class="card feat"><svg viewBox="0 0 24 24"><path d="M4 20V10M10 20V4M16 20v-7M22 20H2"/></svg><h3>إحصائيات القناة</h3><p>اربط قناتك لعرض المشتركين والمشاهدات لاحقاً.</p></div>
</div></div></section>

<footer><div class="wrap">© 2026 NEURA STUDIO — جميع الحقوق محفوظة</div></footer>

<!-- نافذة ربط القناة -->
<div class="ov" id="ov" role="dialog" aria-modal="true" aria-labelledby="mt"><div class="md">
 <h3 id="mt">اربط قناتك على يوتيوب</h3>
 <!-- data-channel-input -->
 <input id="in" type="url" placeholder="الصق رابط قناتك هنا" aria-label="رابط القناة">
 <div class="err" id="er"></div>
 <small>سيتم حفظ الرابط محلياً في متصفحك</small>
 <div class="row"><button class="btn" id="ok">ربط</button><button class="btn ghost" id="un" hidden>فك الربط</button><button class="btn ghost" id="no">إلغاء</button></div>
</div></div>
<div id="toast" role="status"></div>

<script type="module">
// ===== إعدادات =====
const CFG={key:'neura.channel'};
const $=s=>document.querySelector(s);
const store={get:()=>{try{return localStorage.getItem(CFG.key)||''}catch{return ''}},set:v=>{try{v?localStorage.setItem(CFG.key,v):localStorage.removeItem(CFG.key)}catch{}}};
// ===== إشعار =====
const toast=t=>{const e=$('#toast');e.textContent=t;e.classList.add('on');setTimeout(()=>e.classList.remove('on'),2800)};
// ===== الوضع =====
$('#th').onclick=()=>{const d=document.documentElement;d.dataset.theme=d.dataset.theme==='light'?'dark':'light'};
document.documentElement.dataset.theme='dark';
// ===== شريط التنقل =====
addEventListener('scroll',()=>$('#nav').classList.toggle('s',scrollY>30),{passive:true});
// ===== تأثير الموجة على الأزرار =====
document.addEventListener('click',e=>{const b=e.target.closest('.btn');if(!b)return;const r=b.getBoundingClientRect(),s=document.createElement('span'),z=Math.max(r.width,r.height);s.className='rip';s.style.cssText=`width:${z}px;height:${z}px;left:${e.clientX-r.left-z/2}px;top:${e.clientY-r.top-z/2}px`;b.append(s);setTimeout(()=>s.remove(),600)});
// ===== نظام ربط القناة =====
const ov=$('#ov'),inp=$('#in');
const yt='<svg width="16" height="16" viewBox="0 0 24 24" fill="#FF0000"><path d="M23 7.2a3 3 0 0 0-2.1-2.1C19 4.6 12 4.6 12 4.6s-7 0-8.9.5A3 3 0 0 0 1 7.2C.5 9 .5 12 .5 12s0 3 .5 4.8a3 3 0 0 0 2.1 2.1c1.9.5 8.9.5 8.9.5s7 0 8.9-.5a3 3 0 0 0 2.1-2.1c.5-1.8.5-4.8.5-4.8s0-3-.5-4.8zM9.8 15.5v-7l6 3.5z"/></svg>';
function render(){const u=store.get();
 $('#lk').innerHTML=u?yt+' قناتي':'⭐ ربط القناة';
 $('#hb').innerHTML=u?'زيارة القناة':'ربط القناة';
 $('#hb').dataset.open=u?'':'modal';$('#hb').href=u||'#';$('#hb').target=u?'_blank':'';$('#hb').rel='noopener';
 $('#em').hidden=!!u;$('#un').hidden=!u;inp.value=u}
const open=()=>{ov.classList.add('on');$('#er').textContent='';inp.classList.remove('bad');inp.focus()};
const close=()=>ov.classList.remove('on');
document.addEventListener('click',e=>{const t=e.target.closest('[data-open=modal]');if(t){e.preventDefault();open()}});
$('#no').onclick=close;ov. uonclick=e=>{if(e.target===ov)close()};
addEventListener('keydown',e=>{if(e.key==='Escape')close()});
$('#ok').onclick=()=>{const v=inp.value.trim();
 let ok=false;try{const u=new URL(v);ok=/(^|\.)(youtube\.com|youtu\.be)$/.test(u.hostname)}catch{}
 if(!ok){inp.classList.add('bad');$('#er').textContent='الرابط غير صالح. الصق رابط قناة يوتيوب يبدأ بـ https://youtube.com';return}
 store.set(v);render();close();toast('تم ربط القناة بنجاح ✅')};
$('#un').onclick=()=>{store.set('');render();close();toast('تم فك ربط القناة')};
render();
// ===== الكتابة المتحركة =====
const w='صانع محتوى الذكاء الاصطناعي';let i=0;
(function tp(){$('#ty').textContent=w.slice(0,i++);if(i<=w.length)setTimeout(tp,70)})();
// ===== بطاقات الفيديو (placeholder) =====
const V=['كيف يغيّر الذكاء الاصطناعي صناعة الأفلام','أفضل أدوات الذكاء الاصطناعي هذا العام','صناعة فيديو كامل بالذكاء الاصطناعي','مستقبل الوظائف مع الذكاء الاصطناعي','شرح النماذج اللغوية للمبتدئين','أتمتة العمل اليومي خطوة بخطوة'];
$('#vg').innerHTML=V.map((t,k)=>`<a class="card vid" href="#" data-api-slot="video-${k}"><div class="th" style="filter:hue-rotate(${k*35}deg)"><svg width="44" height="44" viewBox="0 0 24 24" fill="#fff"><path d="m9 6 10 6-10 6z"/></svg><i>${7+k*2}:${10+k*7}</i></div><h3>${t}</h3><p>قريباً — سيتم ملؤها من قناتك</p></a>`).join('');
// ===== عدّاد الأرقام =====
const io=new IntersectionObserver(es=>es.forEach(e=>{if(!e.isIntersecting)return;io.unobserve(e.target);const el=e.target,n=+el.dataset.n,t0=performance.now();(function f(t){const p=Math.min((t-t0)/1200,1);el.textContent=Math.round(n*p).toLocaleString('en');if(p<1)requestAnimationFrame(f)})(t0)}));
document.querySelectorAll('[data-n]').forEach(e=>io.observe(e));
// ===== الجسيمات =====
const cv=$('#pc'),cx=cv.getContext('2d');let P=[];
const rs=()=>{cv.width=cv.offsetWidth;cv.height=cv.offsetHeight;P=Array.from({length:Math.min(70,cv.width/14)},()=>({x:Math.random()*cv.width,y:Math.random()*cv.height,vx:Math.random()-.5,vy:Math.random()-.5}))};
rs();addEventListener('resize',rs);
(function dr(){cx.clearRect(0,0,cv.width,cv.height);P.forEach((p,a)=>{p.x=(p.x+p.vx+cv.width)%cv.width;p.y=(p.y+p.vy+cv.height)%cv.height;cx.fillStyle='rgba(139,92,246,.7)';cx.fillRect(p.x,p.y,2,2);for(let b=a+1;b<P.length;b++){const d=Math.hypot(p.x-P[b].x,p.y-P[b].y);if(d<110){cx.strokeStyle=`rgba(6,182,212,${.18*(1-d/110)})`;cx.beginPath();cx.moveTo(p.x,p.y);cx.lineTo(P[b].x,P[b].y);cx.stroke()}}});requestAnimationFrame(dr)})();
addEventListener('load',()=>setTimeout(()=>$('#ld').classList.add('off'),500));
</script>
</body>
</html>
