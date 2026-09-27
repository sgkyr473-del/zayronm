<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>پنل و چیت ZAYRON | @panel_chit_zayron</title>

<meta name="description"
content="پنل و چیت ZAYRON - مرجع اختصاصی محتوا، پنل، چیت و سنسی ZAYRON">

<style>

/* =========================
   RESET
========================= */

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:
        Tahoma,
        Arial,
        sans-serif;
}

html{
    scroll-behavior:smooth;
}

body{
    min-height:100vh;
    color:#fff;
    background:
        radial-gradient(
            circle at 15% 15%,
            rgba(0,150,255,.20),
            transparent 28%
        ),
        radial-gradient(
            circle at 85% 75%,
            rgba(70,0,255,.18),
            transparent 30%
        ),
        #02060c;
    overflow-x:hidden;
}


/* =========================
   BACKGROUND GRID
========================= */

body::before{
    content:"";
    position:fixed;
    inset:0;
    z-index:-3;

    background-image:
        linear-gradient(
            rgba(0,174,255,.035) 1px,
            transparent 1px
        ),
        linear-gradient(
            90deg,
            rgba(0,174,255,.035) 1px,
            transparent 1px
        );

    background-size:45px 45px;

    mask-image:
        linear-gradient(
            to bottom,
            black,
            transparent
        );
}


/* =========================
   GLOW ORBS
========================= */

.orb{
    position:fixed;
    border-radius:50%;
    filter:blur(70px);
    opacity:.18;
    pointer-events:none;
    z-index:-2;
}

.orb1{
    width:230px;
    height:230px;
    background:#008cff;
    top:12%;
    left:-80px;
    animation:float1 8s infinite alternate ease-in-out;
}

.orb2{
    width:260px;
    height:260px;
    background:#572cff;
    right:-100px;
    bottom:10%;
    animation:float2 10s infinite alternate ease-in-out;
}

@keyframes float1{
    from{
        transform:translateY(0);
    }
    to{
        transform:translateY(80px);
    }
}

@keyframes float2{
    from{
        transform:translateY(0);
    }
    to{
        transform:translateY(-90px);
    }
}


/* =========================
   CONTAINER
========================= */

.container{
    width:min(1120px,92%);
    margin:auto;
}


/* =========================
   HEADER
========================= */

header{
    padding:20px 0;
    position:relative;
    z-index:10;
}

.navbar{
    display:flex;
    justify-content:space-between;
    align-items:center;

    padding:15px 20px;

    border:
        1px solid
        rgba(0,190,255,.28);

    border-radius:20px;

    background:
        rgba(4,13,24,.72);

    backdrop-filter:blur(18px);

    box-shadow:
        0 0 35px
        rgba(0,150,255,.08);
}

.logo{
    color:#18baff;
    font-size:22px;
    font-weight:900;

    text-shadow:
        0 0 10px #009dff,
        0 0 25px #006eff;

    letter-spacing:1px;
}

.nav-text{
    color:#7e9bad;
    font-size:12px;
}


/* =========================
   HERO
========================= */

.hero{
    min-height:78vh;

    display:flex;
    align-items:center;
    justify-content:center;

    text-align:center;

    position:relative;
}

.hero-content{
    max-width:850px;
}

.badge{
    display:inline-block;

    padding:9px 18px;

    border:
        1px solid
        rgba(0,190,255,.35);

    border-radius:50px;

    color:#28c4ff;

    background:
        rgba(0,150,255,.08);

    font-size:12px;

    box-shadow:
        0 0 20px
        rgba(0,170,255,.08);

    margin-bottom:22px;
}

.hero h1{
    font-size:
        clamp(42px,9vw,92px);

    font-weight:1000;

    line-height:1.15;

    color:#fff;

    text-shadow:
        0 0 10px #00aaff,
        0 0 30px #0077ff,
        0 0 70px
        rgba(0,140,255,.45);
}

.hero h2{
    margin-top:15px;

    color:#16bfff;

    font-size:
        clamp(22px,4vw,38px);

    text-shadow:
        0 0 15px
        rgba(0,180,255,.55);
}

.hero p{
    max-width:700px;

    margin:
        22px auto 0;

    color:#91a7b8;

    line-height:2;

    font-size:14px;
}


/* =========================
   BUTTONS
========================= */

.buttons{
    display:flex;
    justify-content:center;
    align-items:center;

    gap:13px;

    flex-wrap:wrap;

    margin-top:30px;
}

.btn{
    display:inline-flex;

    align-items:center;
    justify-content:center;

    min-width:175px;

    padding:14px 24px;

    border-radius:14px;

    text-decoration:none;

    color:white;

    font-size:14px;
    font-weight:bold;

    border:
        1px solid
        rgba(0,200,255,.5);

    background:
        linear-gradient(
            135deg,
            #009dff,
            #0057dc
        );

    box-shadow:
        0 0 25px
        rgba(0,140,255,.22);

    transition:.25s;
}

.btn:hover{
    transform:
        translateY(-5px)
        scale(1.02);

    box-shadow:
        0 0 35px
        rgba(0,175,255,.5);
}

.btn.secondary{
    background:
        rgba(255,255,255,.035);
}


/* =========================
   SECTION
========================= */

.section{
    padding:80px 0;
}

.section-title{
    text-align:center;
    margin-bottom:38px;
}

.section-title h2{
    font-size:30px;

    color:#fff;

    text-shadow:
        0 0 15px
        rgba(0,170,255,.25);
}

.section-title p{
    color:#718899;

    font-size:13px;

    margin-top:10px;
}


/* =========================
   CARDS
========================= */

.cards{
    display:grid;

    grid-template-columns:
        repeat(3,1fr);

    gap:18px;
}

.card{
    position:relative;

    padding:28px 22px;

    min-height:210px;

    border-radius:22px;

    border:
        1px solid
        rgba(0,185,255,.18);

    background:
        linear-gradient(
            145deg,
            rgba(10,30,48,.82),
            rgba(4,10,18,.80)
        );

    backdrop-filter:blur(14px);

    overflow:hidden;

    transition:.3s;
}

.card::before{
    content:"";

    position:absolute;

    top:0;
    right:0;
    left:0;

    height:1px;

    background:
        linear-gradient(
            90deg,
            transparent,
            #08baff,
            transparent
        );

    opacity:.7;
}

.card:hover{
    transform:translateY(-8px);

    border-color:
        rgba(0,195,255,.55);

    box-shadow:
        0 18px 50px
        rgba(0,130,255,.13);
}

.icon{
    width:52px;
    height:52px;

    display:flex;

    align-items:center;
    justify-content:center;

    border-radius:16px;

    background:
        rgba(0,170,255,.10);

    border:
        1px solid
        rgba(0,190,255,.18);

    font-size:23px;

    margin-bottom:18px;

    box-shadow:
        inset 0 0 20px
        rgba(0,160,255,.04);
}

.card h3{
    font-size:18px;

    color:#fff;

    margin-bottom:12px;
}

.card p{
    color:#8198a9;

    line-height:1.9;

    font-size:13px;
}


/* =========================
   MAIN BRAND CARD
========================= */

.brand-box{
    position:relative;

    padding:45px 25px;

    text-align:center;

    border-radius:28px;

    border:
        1px solid
        rgba(0,190,255,.28);

    background:
        linear-gradient(
            135deg,
            rgba(0,125,255,.11),
            rgba(50,0,255,.09)
        );

    backdrop-filter:blur(15px);

    overflow:hidden;

    box-shadow:
        0 0 55px
        rgba(0,130,255,.07);
}

.brand-box::after{
    content:"";

    position:absolute;

    width:250px;
    height:250px;

    border-radius:50%;

    background:
        rgba(0,160,255,.08);

    filter:blur(50px);

    top:-120px;
    left:-80px;
}

.brand-small{
    color:#24bfff;

    font-size:11px;

    letter-spacing:2px;
}

.brand-name{
    margin:15px 0;

    color:#fff;

    font-size:
        clamp(27px,6vw,48px);

    font-weight:1000;

    text-shadow:
        0 0 15px #008cff,
        0 0 35px
        rgba(0,130,255,.45);
}

.brand-id{
    color:#18baff;

    font-size:18px;

    direction:ltr;

    margin-bottom:15px;
}

.brand-box p{
    max-width:650px;

    margin:auto;

    color:#879eae;

    line-height:2;

    font-size:13px;
}


/* =========================
   STATS
========================= */

.stats{
    display:grid;

    grid-template-columns:
        repeat(3,1fr);

    gap:15px;

    margin-top:20px;
}

.stat{
    text-align:center;

    padding:23px 10px;

    border-radius:18px;

    border:
        1px solid
        rgba(255,255,255,.06);

    background:
        rgba(255,255,255,.025);
}

.stat strong{
    display:block;

    color:#1bbcff;

    font-size:25px;

    margin-bottom:6px;

    text-shadow:
        0 0 12px
        rgba(0,170,255,.4);
}

.stat span{
    color:#718898;

    font-size:11px;
}


/* =========================
   CTA
========================= */

.cta{
    text-align:center;

    padding:40px 20px;

    border-radius:25px;

    background:
        rgba(0,130,255,.055);

    border:
        1px solid
        rgba(0,170,255,.15);
}

.cta h2{
    color:#fff;

    margin-bottom:12px;
}

.cta p{
    color:#8197a8;

    font-size:13px;

    margin-bottom:5px;
}


/* =========================
   FOOTER
========================= */

footer{
    padding:40px 0;

    text-align:center;

    border-top:
        1px solid
        rgba(255,255,255,.05);

    color:#607584;

    font-size:12px;
}

footer .footer-brand{
    color:#18baff;

    font-size:17px;

    font-weight:bold;

    margin-bottom:8px;
}

footer .footer-id{
    direction:ltr;

    margin-top:8px;

    color:#758c9d;
}


/* =========================
   MOBILE
========================= */

@media(max-width:750px){

    .navbar{
        padding:14px 15px;
    }

    .logo{
        font-size:18px;
    }

    .nav-text{
        display:none;
    }

    .hero{
        min-height:70vh;
    }

    .hero h1{
        letter-spacing:3px;
    }

    .cards{
        grid-template-columns:1fr;
    }

    .stats{
        grid-template-columns:1fr;
    }

    .section{
        padding:60px 0;
    }

    .btn{
        width:100%;
        max-width:300px;
    }

}


/* =========================
   REDUCED MOTION
========================= */

@media(prefers-reduced-motion:reduce){

    *,
    *::before,
    *::after{
        animation:none !important;
        transition:none !important;
        scroll-behavior:auto !important;
    }

}

</style>
</head>


<body>

<!-- BACKGROUND -->
<div class="orb orb1"></div>
<div class="orb orb2"></div>


<!-- HEADER -->

<header>

<div class="container">

<div class="navbar">

<div class="logo">
پنل و چیت ZAYRON
</div>

<div class="nav-text">
@panel_chit_zayron
</div>

</div>

</div>

</header>



<!-- HERO -->

<section class="hero">

<div class="container hero-content">

<div class="badge">
⚡ مرجع پنل و چیت ZAYRON
</div>

<h1>
پنل و چیت
</h1>

<h2>
ZAYRON
</h2>

<p>
به سایت رسمی پنل و چیت ZAYRON خوش آمدید؛
مرجع اختصاصی برای معرفی پنل‌ها، چیت‌ها،
سنسی، تنظیمات و جدیدترین محتوای ZAYRON.
</p>


<div class="buttons">

<a
class="btn"
href="https://rubika.ir/panel_chit_zayron"
target="_blank">

🔵 روبیکا

</a>


<a
class="btn secondary"
href="https://t.me/panel_chit_zayron"
target="_blank">

✈️ تلگرام

</a>

</div>

</div>

</section>



<!-- FEATURES -->

<section class="section">

<div class="container">

<div class="section-title">

<h2>
پنل و چیت ZAYRON
</h2>

<p>
همه‌چیز در یک مرجع
</p>

</div>


<div class="cards">


<div class="card">

<div class="icon">
🎯
</div>

<h3>
پنل ZAYRON
</h3>

<p>
معرفی پروژه‌ها و پنل‌های ZAYRON
با رابط کاربری مدرن و گیمینگ.
</p>

</div>



<div class="card">

<div class="icon">
⚡
</div>

<h3>
چیت ZAYRON
</h3>

<p>
دسترسی به جدیدترین مطالب و
اطلاعات منتشرشده درباره چیت‌های ZAYRON.
</p>

</div>



<div class="card">

<div class="icon">
🔥
</div>

<h3>
سنسی ZAYRON
</h3>

<p>
محتوای مربوط به سنسی و تنظیمات
گیمینگ ZAYRON را دنبال کنید.
</p>

</div>


</div>

</div>

</section>



<!-- OFFICIAL BRAND -->

<section class="section">

<div class="container">

<div class="brand-box">

<div class="brand-small">
OFFICIAL ZAYRON
</div>

<div class="brand-name">
پنل و چیت ZAYRON
</div>

<div class="brand-id">
@panel_chit_zayron
</div>

<p>
جدیدترین مطالب، پروژه‌ها، پنل‌ها،
چیت‌ها و محتوای ZAYRON را از
کانال‌های ما دنبال کنید.
</p>


<div class="buttons">

<a
class="btn"
href="https://rubika.ir/panel_chit_zayron"
target="_blank">

ورود به پنل و چیت ZAYRON در روبیکا

</a>


<a
class="btn secondary"
href="https://t.me/panel_chit_zayron"
target="_blank">

ورود به پنل و چیت ZAYRON در تلگرام

</a>

</div>

</div>


<div class="stats">

<div class="stat">

<strong>
ZAYRON
</strong>

<span>
پنل و چیت
</span>

</div>


<div class="stat">

<strong>
24/7
</strong>

<span>
محتوای ZAYRON
</span>

</div>


<div class="stat">

<strong>
PRO
</strong>

<span>
طراحی و محتوا
</span>

</div>

</div>

</div>

</section>



<!-- CTA -->

<section class="section">

<div class="container">

<div class="cta">

<h2>
پنل و چیت ZAYRON را دنبال کن
</h2>

<p>
برای دریافت جدیدترین محتوای ZAYRON
کانال ما را دنبال کنید.
</p>

<div class="buttons">

<a
class="btn"
href="https://rubika.ir/panel_chit_zayron"
target="_blank">

🔵 کانال روبیکا

</a>


<a
class="btn secondary"
href="https://t.me/panel_chit_zayron"
target="_blank">

✈️ کانال تلگرام

</a>

</div>

</div>

</div>

</section>



<!-- FOOTER -->

<footer>

<div class="container">

<div class="footer-brand">
پنل و چیت ZAYRON
</div>

<div>
مرجع محتوای پنل و چیت ZAYRON
</div>

<div class="footer-id">
@panel_chit_zayron
</div>

</div>

</footer>


</body>
</html>
