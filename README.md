```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>ALL IN ONE | RV CREATION</title>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&family=Space+Grotesk:wght@500;600;700&display=swap" rel="stylesheet">

<style>

/* =========================================================
   GLOBAL
========================================================= */

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

html{
    scroll-behavior:smooth;
}

body{
    min-height:100vh;
    font-family:Arial,Inter,sans-serif;
    background:
        radial-gradient(circle at 10% 10%,rgba(0,234,255,.10),transparent 25%),
        radial-gradient(circle at 90% 20%,rgba(139,92,246,.13),transparent 25%),
        #07101f;
    color:white;
}

:root{
    --bg:#07101f;
    --panel:#101a31;
    --panel2:#151f39;
    --text:#ffffff;
    --muted:#98a6c4;
    --border:#2a385d;
    --cyan:#00eaff;
    --purple:#8b5cf6;
    --green:#20d0bd;
}


/* =========================================================
   HEADER
========================================================= */

header{
    width:100%;
    min-height:80px;
    padding:12px 25px;

    display:flex;
    justify-content:space-between;
    align-items:center;

    position:sticky;
    top:0;
    z-index:1000;

    background:rgba(10,20,38,.94);
    border-bottom:1px solid var(--border);

    backdrop-filter:blur(18px);
}

.brand{
    display:flex;
    align-items:center;
    gap:12px;
    cursor:pointer;
}

.rv-logo{
    width:52px;
    height:52px;

    display:flex;
    justify-content:center;
    align-items:center;

    border-radius:15px;

    background:linear-gradient(
        135deg,
        #00eaff,
        #8b5cf6
    );

    color:white;
    font-size:21px;
    font-weight:900;

    box-shadow:
        0 0 15px rgba(0,234,255,.35),
        0 0 30px rgba(139,92,246,.25);

    transition:.3s;
}

.rv-logo:hover{
    transform:scale(1.08) rotate(-5deg);
}

.brand-text{
    display:flex;
    flex-direction:column;
}

.brand-text h2{
    font-size:20px;
    letter-spacing:1px;
}

.brand-text h2 span{
    color:var(--cyan);
}

.brand-text small{
    color:var(--muted);
    font-size:9px;
    letter-spacing:2px;
    margin-top:4px;
}

.clock{
    color:var(--cyan);
    font-size:15px;
    font-weight:bold;
}


/* =========================================================
   MAIN
========================================================= */

.container{
    width:95%;
    max-width:1450px;
    margin:25px auto;
}

.welcome{
    text-align:center;
    margin-bottom:30px;
}

.welcome h1{
    font-size:42px;
    margin-bottom:8px;

    background:
        linear-gradient(
            90deg,
            white,
            #00eaff,
            #8b5cf6
        );

    -webkit-background-clip:text;
    -webkit-text-fill-color:transparent;
}

.welcome p{
    color:var(--muted);
    font-size:15px;
    line-height:1.7;
}


/* =========================================================
   APP GRID
========================================================= */

.apps{
    display:grid;
    grid-template-columns:
        repeat(auto-fit,minmax(145px,1fr));
    gap:15px;
    margin-bottom:25px;
}

.app-card{
    background:var(--panel);
    border:1px solid var(--border);
    border-radius:18px;
    padding:20px 10px;
    text-align:center;
    cursor:pointer;
    transition:.3s;
}

.app-card:hover{
    transform:translateY(-6px);
    border-color:var(--cyan);
    box-shadow:
        0 0 25px rgba(0,234,255,.16);
}

.icon{
    width:60px;
    height:60px;
    margin:0 auto 12px;

    border-radius:17px;

    display:flex;
    justify-content:center;
    align-items:center;

    font-size:25px;
    font-weight:bold;
}

.instagram{
    background:linear-gradient(
        135deg,
        #833ab4,
        #fd1d1d,
        #fcb045
    );
}

.facebook{
    background:#1877f2;
}

.spotify{
    background:#1db954;
}

.flipkart{
    background:#2874f0;
}

.whatsapp{
    background:#25d366;
}

.amazon{
    background:#ff9900;
    color:#111;
}

.maps{
    background:#34a853;
}

.age{
    background:linear-gradient(
        135deg,
        #ff9966,
        #ff5e62
    );
}

.resume{
    background:linear-gradient(
        135deg,
        #805ef8,
        #20cdbf
    );
}

.app-card h3{
    font-size:15px;
    margin-bottom:5px;
}

.app-card p{
    color:var(--muted);
    font-size:11px;
}


/* =========================================================
   CONTENT
========================================================= */

.content{
    min-height:650px;
    background:var(--panel);
    border:1px solid var(--border);
    border-radius:20px;
    overflow:hidden;
}

.content-header{
    padding:15px 20px;
    background:var(--panel2);
    border-bottom:1px solid var(--border);

    display:flex;
    justify-content:space-between;
    align-items:center;
}

.content-header h2{
    font-size:18px;
}

.open-btn{
    border:none;
    background:var(--cyan);
    color:#001219;
    font-weight:bold;
    padding:10px 16px;
    border-radius:10px;
    cursor:pointer;
}

.open-btn:hover{
    opacity:.85;
}


/* =========================================================
   HOME
========================================================= */

.home{
    min-height:590px;

    display:flex;
    flex-direction:column;
    align-items:center;
    justify-content:center;

    text-align:center;
    padding:30px;
}

.home-icon{
    font-size:80px;
    margin-bottom:20px;
}

.home h2{
    font-size:30px;
    margin-bottom:12px;
}

.home p{
    max-width:720px;
    color:var(--muted);
    line-height:1.8;
}


/* =========================================================
   AGE FINDER
========================================================= */

.age-container{
    padding:25px;
}

.age-form{
    max-width:850px;
    margin:auto;

    display:grid;
    grid-template-columns:repeat(2,1fr);
    gap:15px;
}

.age-group{
    display:flex;
    flex-direction:column;
    gap:7px;
}

.age-group label{
    color:var(--muted);
    font-size:13px;
}

.age-group input{
    padding:13px;
    background:var(--panel2);
    color:white;

    border:1px solid var(--border);
    border-radius:10px;

    outline:none;
}

.full{
    grid-column:1/-1;
}

.age-button{
    width:100%;
    padding:14px;

    border:none;
    border-radius:10px;

    background:
        linear-gradient(
            90deg,
            #00eaff,
            #8b5cf6
        );

    color:white;
    font-weight:bold;
    cursor:pointer;
}

.age-result{
    max-width:850px;
    margin:25px auto 0;
}

.age-main{
    padding:20px;
    background:var(--panel2);
    border:1px solid var(--border);
    border-radius:15px;
    text-align:center;
}

.age-main h3{
    color:var(--cyan);
    font-size:30px;
    margin-bottom:8px;
}

.age-main p{
    color:var(--muted);
}

.age-grid{
    display:grid;
    grid-template-columns:repeat(4,1fr);
    gap:12px;
    margin-top:15px;
}

.age-box{
    padding:18px;
    background:var(--panel2);
    border:1px solid var(--border);
    border-radius:13px;
    text-align:center;
    color:var(--muted);
}

.age-box strong{
    display:block;
    color:var(--cyan);
    font-size:27px;
    margin-bottom:5px;
}

.birthday-box{
    margin-top:15px;
    padding:18px;
    background:var(--panel2);
    border:1px solid var(--border);
    border-radius:13px;
    text-align:center;
    color:var(--muted);
}

.birthday-box strong{
    color:var(--cyan);
}


/* =========================================================
   MAP
========================================================= */

.map-container{
    padding:20px;
}

.map-search{
    display:flex;
    gap:10px;
    margin-bottom:15px;
}

.map-search input{
    flex:1;
    padding:13px;
    background:var(--panel2);
    color:white;
    border:1px solid var(--border);
    border-radius:10px;
    outline:none;
}

.map-search button{
    padding:0 20px;
    border:none;
    border-radius:10px;
    background:var(--cyan);
    color:#001219;
    font-weight:bold;
    cursor:pointer;
}

iframe{
    width:100%;
    height:560px;
    border:none;
    background:white;
}


/* =========================================================
   NOVACV
========================================================= */

.cv-page{
    padding:25px;
    background:
        radial-gradient(
            circle at top left,
            rgba(124,92,255,.10),
            transparent 35%
        );
}

.cv-hero{
    max-width:1100px;
    margin:0 auto 35px;
}

.eyebrow,
.kicker{
    font-size:11px;
    letter-spacing:.17em;
    color:#a99cff;
    font-weight:800;
}

.cv-hero h1{
    font-family:"Space Grotesk",Arial,sans-serif;
    font-size:clamp(40px,6vw,70px);
    line-height:1;
    margin:15px 0 20px;
}

.cv-hero h1 span{
    background:
        linear-gradient(
            90deg,
            #9d8cff,
            #43e0d3
        );

    -webkit-background-clip:text;
    background-clip:text;
    color:transparent;
}

.cv-hero p{
    max-width:760px;
    color:var(--muted);
    font-size:17px;
    line-height:1.7;
}

.hero-stats{
    display:flex;
    gap:10px;
    flex-wrap:wrap;
    margin-top:22px;
}

.hero-stats span{
    padding:9px 13px;
    border:1px solid var(--border);
    border-radius:999px;
    background:rgba(255,255,255,.03);
    color:#cddaf0;
    font-size:12px;
}

.cv-workspace,
.cv-insights,
.cv-jobs,
.cv-how{
    max-width:1100px;
    margin:0 auto 22px;
}

.cv-workspace{
    display:grid;
    grid-template-columns:1.15fr .85fr;
    gap:20px;
}

.cv-panel{
    border:1px solid var(--border);
    background:rgba(11,23,40,.76);
    backdrop-filter:blur(20px);
    border-radius:22px;
    padding:22px;
    box-shadow:0 20px 45px rgba(0,0,0,.2);
}

.panel-head{
    display:flex;
    align-items:flex-start;
    justify-content:space-between;
    gap:15px;
}

.cv-panel h2{
    font-family:"Space Grotesk",Arial,sans-serif;
    font-size:24px;
    margin:5px 0;
}

.muted{
    color:var(--muted);
}

.secure{
    font-size:10px;
    color:#9fe7da;
    border:1px solid rgba(24,213,195,.22);
    background:rgba(24,213,195,.06);
    border-radius:999px;
    padding:7px 9px;
}

.dropzone{
    border:1px dashed #4c5f79;
    border-radius:18px;

    min-height:200px;
    margin-top:18px;

    display:flex;
    flex-direction:column;
    justify-content:center;
    align-items:center;

    text-align:center;
    cursor:pointer;

    background:
        linear-gradient(
            180deg,
            rgba(124,92,255,.05),
            rgba(24,213,195,.02)
        );
}

.dropzone.drag{
    border-color:#a99cff;
    background:rgba(124,92,255,.09);
}

.upload-icon{
    width:54px;
    height:54px;
    border-radius:16px;
    background:rgba(124,92,255,.16);

    display:grid;
    place-items:center;

    font-size:30px;
    margin-bottom:12px;
}

.dropzone strong{
    font-size:17px;
}

.dropzone small,
.dropzone em{
    display:block;
    color:var(--muted);
    margin-top:5px;
    font-style:normal;
}

.file-row{
    display:flex;
    justify-content:space-between;
    align-items:center;
    margin-top:12px;
    padding:10px 12px;

    border:1px solid var(--border);
    border-radius:12px;
}

.mini,
.secondary{
    border:1px solid var(--border);
    background:rgba(255,255,255,.04);
    color:#dbe7f7;
    border-radius:10px;
    padding:9px 13px;
    cursor:pointer;
}

.or{
    display:flex;
    align-items:center;
    gap:10px;

    color:#65768d;
    font-size:11px;

    margin:18px 0;
}

.or:before,
.or:after{
    content:"";
    height:1px;
    background:var(--border);
    flex:1;
}

.cv-panel textarea{
    width:100%;
    min-height:130px;
    resize:vertical;

    background:rgba(4,10,19,.55);
    border:1px solid var(--border);

    color:#eaf1fb;

    border-radius:15px;
    padding:14px;

    font:14px/1.6 Inter,Arial;
    outline:none;
}

.cv-panel textarea:focus{
    border-color:#6651e9;
}

.actions{
    display:flex;
    gap:10px;
    margin-top:13px;
}

.primary{
    flex:1;
    border:0;
    border-radius:13px;
    padding:14px 16px;

    color:white;
    font-weight:800;

    background:
        linear-gradient(
            135deg,
            #805ef8,
            #20cdbf
        );

    cursor:pointer;
}

.status{
    min-height:20px;
    color:#9fb0c6;
    font-size:12px;
    margin-top:9px;
}

.score-panel{
    display:flex;
    flex-direction:column;
}

.score-wrap{
    display:flex;
    gap:18px;
    align-items:center;
    margin:20px 0;
}

.ring{
    width:150px;
    height:150px;

    border-radius:50%;

    display:grid;
    place-items:center;

    background:
        conic-gradient(
            #8c72ff 0deg,
            #8c72ff 0deg,
            #1a2940 0deg 360deg
        );

    position:relative;
    flex:none;
}

.ring:after{
    content:"";
    position:absolute;
    inset:12px;
    border-radius:50%;
    background:#0b1728;
}

.ring>div{
    position:relative;
    z-index:1;
    text-align:center;
}

.ring strong{
    font:800 42px "Space Grotesk";
}

.ring span{
    color:#8193ab;
}

.score-label{
    font-weight:800;
    font-size:18px;
}

.score-wrap p{
    color:var(--muted);
    line-height:1.55;
    font-size:13px;
}

.mini-grid{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:10px;
    margin-top:auto;
}

.mini-grid>div{
    border:1px solid var(--border);
    padding:13px;
    border-radius:14px;
    background:rgba(255,255,255,.025);
}

.mini-grid b{
    display:block;
    font-size:22px;
}

.mini-grid span{
    color:var(--muted);
    font-size:11px;
}

.cv-insights{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:20px;
}

.pill{
    font-size:11px;
    border:1px solid rgba(24,213,195,.25);
    background:rgba(24,213,195,.06);
    padding:7px 10px;
    border-radius:999px;
    color:#92e9de;
}

.pill.warn{
    border-color:rgba(255,183,74,.25);
    color:#ffd08d;
    background:rgba(255,183,74,.06);
}

.chips{
    display:flex;
    flex-wrap:wrap;
    gap:8px;
    margin-top:20px;
}

.chip{
    padding:8px 10px;
    border-radius:999px;
    background:rgba(124,92,255,.12);
    border:1px solid rgba(124,92,255,.28);
    color:#d8d0ff;
    font-size:12px;
}

.empty{
    color:#71849d;
    padding:30px 0;
}

.gap-list{
    margin-top:15px;
}

.gap{
    display:flex;
    justify-content:space-between;
    align-items:center;

    padding:14px 0;
    border-bottom:1px solid var(--border);
}

.gap:last-child{
    border-bottom:0;
}

.gap b{
    font-size:13px;
}

.gap span{
    font-size:11px;
    color:#ffca7a;
}

.list{
    margin-top:10px;
}

.list-item{
    display:flex;
    gap:10px;
    padding:12px 0;

    border-bottom:1px solid var(--border);

    color:#cbd8e9;
    line-height:1.5;
    font-size:13px;
}

.list-item:last-child{
    border-bottom:0;
}

.dot{
    width:9px;
    height:9px;
    border-radius:50%;
    background:#43e0d3;
    flex:none;
    margin-top:5px;
}

.numbered .num{
    width:24px;
    height:24px;

    border-radius:8px;

    background:rgba(124,92,255,.16);

    display:grid;
    place-items:center;

    color:#c8bfff;
    font-size:11px;
    font-weight:800;

    flex:none;
}

.cv-jobs{
    margin-bottom:40px;
}

.jobs-grid{
    display:grid;
    grid-template-columns:repeat(2,1fr);
    gap:14px;
    margin-top:18px;
}

.job{
    border:1px solid var(--border);
    border-radius:18px;
    padding:18px;
    background:rgba(255,255,255,.025);
}

.job-top{
    display:flex;
    justify-content:space-between;
    gap:10px;
}

.job h3{
    margin:0;
    font-size:16px;
}

.job small{
    color:var(--muted);
}

.match{
    font-weight:800;
    font-size:15px;
}

.bar{
    height:7px;
    border-radius:999px;
    background:#1a2940;
    margin:13px 0;
    overflow:hidden;
}

.bar i{
    display:block;
    height:100%;
    border-radius:inherit;

    background:
        linear-gradient(
            90deg,
            #8060fa,
            #20cdbf
        );
}

.missing{
    font-size:11px;
    color:#9fb0c6;
}

.cv-how{
    display:flex;
    flex-direction:column;
    gap:20px;
    margin-bottom:40px;
}

.cv-how h2{
    font-family:"Space Grotesk";
    font-size:30px;
    margin:8px 0;
}

.steps{
    display:grid;
    grid-template-columns:repeat(4,1fr);
    gap:12px;
}

.steps>div{
    border:1px solid var(--border);
    padding:18px;
    border-radius:17px;
    background:rgba(255,255,255,.025);
}

.steps b{
    font-size:12px;
    color:#9d8cff;
}

.steps h3{
    margin:12px 0 7px;
}

.steps p{
    color:var(--muted);
    font-size:12px;
    line-height:1.5;
    margin:0;
}


/* =========================================================
   FOOTER
========================================================= */

footer{
    text-align:center;
    padding:25px;
    color:var(--muted);
    font-size:13px;
    border-top:1px solid var(--border);
}


/* =========================================================
   MOBILE
========================================================= */

@media(max-width:900px){

    .cv-workspace,
    .cv-insights,
    .jobs-grid{
        grid-template-columns:1fr;
    }

    .steps{
        grid-template-columns:1fr 1fr;
    }
}

@media(max-width:700px){

    header{
        padding:12px 15px;
    }

    .brand-text h2{
        font-size:16px;
    }

    .rv-logo{
        width:44px;
        height:44px;
        font-size:18px;
    }

    .clock{
        display:none;
    }

    .welcome h1{
        font-size:29px;
    }

    .age-form{
        grid-template-columns:1fr;
    }

    .full{
        grid-column:auto;
    }

    .age-grid{
        grid-template-columns:repeat(2,1fr);
    }

    .map-search{
        flex-direction:column;
    }

    .map-search button{
        padding:13px;
    }

    .score-wrap{
        align-items:flex-start;
    }
}

@media(max-width:520px){

    .container{
        width:96%;
    }

    .cv-page{
        padding:16px;
    }

    .steps{
        grid-template-columns:1fr;
    }

    .panel-head{
        flex-direction:column;
    }

    .mini-grid{
        grid-template-columns:1fr 1fr 1fr;
    }

    .ring{
        width:120px;
        height:120px;
    }

    .ring strong{
        font-size:34px;
    }
}

</style>
</head>


<body>


<!-- =========================================================
     HEADER
========================================================= -->

<header>

    <div class="brand" onclick="showHome()">

        <div class="rv-logo">
            RV
        </div>

        <div class="brand-text">

            <h2>
                <span>RV</span> CREATION
            </h2>

            <small>
                ALL IN ONE
            </small>

        </div>

    </div>

    <div class="clock" id="clock">
        00:00:00
    </div>

</header>


<div class="container">


<!-- =========================================================
     TITLE
========================================================= -->

<div class="welcome">

    <h1>
        ALL IN ONE
    </h1>

    <p>
        Social Media • Music • Shopping • Maps • Age Finder •
        AI Resume Analyzer
    </p>

</div>


<!-- =========================================================
     APPLICATIONS
========================================================= -->

<div class="apps">


    <div class="app-card"
         onclick="openExternal('https://www.instagram.com/')">

        <div class="icon instagram">
            ◎
        </div>

        <h3>Instagram</h3>
        <p>Social Media</p>

    </div>


    <div class="app-card"
         onclick="openExternal('https://www.facebook.com/')">

        <div class="icon facebook">
            f
        </div>

        <h3>Facebook</h3>
        <p>Social Media</p>

    </div>


    <div class="app-card"
         onclick="openExternal('https://open.spotify.com/')">

        <div class="icon spotify">
            ♪
        </div>

        <h3>Spotify</h3>
        <p>Music</p>

    </div>


    <div class="app-card"
         onclick="openExternal('https://www.flipkart.com/')">

        <div class="icon flipkart">
            F
        </div>

        <h3>Flipkart</h3>
        <p>Shopping</p>

    </div>


    <div class="app-card"
         onclick="openExternal('https://web.whatsapp.com/')">

        <div class="icon whatsapp">
            ☎
        </div>

        <h3>WhatsApp Web</h3>
        <p>Messaging</p>

    </div>


    <div class="app-card"
         onclick="openExternal('https://www.amazon.in/')">

        <div class="icon amazon">
            a
        </div>

        <h3>Amazon</h3>
        <p>Shopping</p>

    </div>


    <div class="app-card"
         onclick="showMaps()">

        <div class="icon maps">
            ⌖
        </div>

        <h3>Google Maps</h3>
        <p>Location</p>

    </div>


    <div class="app-card"
         onclick="showAgeFinder()">

        <div class="icon age">
            🎂
        </div>

        <h3>Age Finder</h3>
        <p>Age & Time</p>

    </div>


    <!-- NEW NOVACV -->

    <div class="app-card"
         onclick="showResumeAnalyzer()">

        <div class="icon resume">
            CV
        </div>

        <h3>NovaCV AI</h3>
        <p>Resume Analyzer</p>

    </div>

</div>


<!-- =========================================================
     MAIN CONTENT
========================================================= -->

<div class="content">

    <div class="content-header">

        <h2 id="pageTitle">
            Welcome
        </h2>

        <button
            class="open-btn"
            id="openButton"
            onclick="openCurrent()">

            Open

        </button>

    </div>


    <div id="displayArea">

        <div class="home">

            <div class="home-icon">
                🌐
            </div>

            <h2>
                Welcome to ALL IN ONE
            </h2>

            <p>
                RV Creation brings your favorite apps and
                useful tools together in one dashboard.
                Use social media, music, shopping,
                Google Maps, Age Finder and the new
                NovaCV AI Resume Analyzer.
            </p>

        </div>

    </div>

</div>


<footer>

    © 2026 RV CREATION |
    ALL IN ONE

</footer>

</div>


<!-- =========================================================
     JAVASCRIPT
========================================================= -->

<script>

/* =========================================================
   VARIABLES
========================================================= */

let currentURL="";
let birthDate=null;
let ageTimer=null;

let lastResult=null;
let selectedFile=null;


/* =========================================================
   CLOCK
========================================================= */

function updateClock(){

    const now=new Date();

    const hours=String(
        now.getHours()
    ).padStart(2,"0");

    const minutes=String(
        now.getMinutes()
    ).padStart(2,"0");

    const seconds=String(
        now.getSeconds()
    ).padStart(2,"0");

    document.getElementById("clock").innerText=
        `${hours}:${minutes}:${seconds}`;
}

setInterval(updateClock,1000);
updateClock();


/* =========================================================
   OPEN EXTERNAL
========================================================= */

function openExternal(url){

    currentURL=url;

    window.open(
        url,
        "_blank",
        "noopener,noreferrer"
    );
}


/* =========================================================
   HOME
========================================================= */

function showHome(){

    clearAgeTimer();

    currentURL="";

    document.getElementById("pageTitle").innerText=
        "Welcome";

    document.getElementById("openButton").innerText=
        "Open";

    document.getElementById("displayArea").innerHTML=`

        <div class="home">

            <div class="home-icon">
                🌐
            </div>

            <h2>
                Welcome to ALL IN ONE
            </h2>

            <p>
                RV Creation brings your favorite apps
                and useful tools together in one simple
                dashboard.
            </p>

        </div>

    `;
}


/* =========================================================
   GOOGLE MAPS
========================================================= */

function showMaps(){

    clearAgeTimer();

    currentURL=
        "https://www.google.com/maps";

    document.getElementById("pageTitle").innerText=
        "Google Maps";

    document.getElementById("openButton").innerText=
        "Open Maps";

    document.getElementById("displayArea").innerHTML=`

        <div class="map-container">

            <div class="map-search">

                <input
                    type="text"
                    id="mapSearch"
                    placeholder="Search a place..."
                    onkeydown="mapEnter(event)"
                >

                <button onclick="searchMap()">
                    Find
                </button>

            </div>

            <iframe
                id="mapFrame"
                src="https://www.google.com/maps?q=India&output=embed"
                loading="lazy">
            </iframe>

        </div>

    `;
}

function searchMap(){

    const input=
        document.getElementById("mapSearch");

    const place=input.value.trim();

    if(place===""){
        return;
    }

    document.getElementById("mapFrame").src=
        "https://www.google.com/maps?q="+
        encodeURIComponent(place)+
        "&output=embed";
}

function mapEnter(event){

    if(event.key==="Enter"){
        searchMap();
    }
}


/* =========================================================
   AGE FINDER
========================================================= */

function showAgeFinder(){

    clearAgeTimer();

    currentURL="";

    document.getElementById("pageTitle").innerText=
        "Age & Time Finder";

    document.getElementById("openButton").innerText=
        "Calculate";

    document.getElementById("displayArea").innerHTML=`

        <div class="age-container">

            <div class="age-form">

                <div class="age-group">

                    <label>
                        Date of Birth
                    </label>

                    <input
                        type="date"
                        id="dob"
                    >

                </div>


                <div class="age-group">

                    <label>
                        Birth Time
                    </label>

                    <input
                        type="time"
                        id="birthTime"
                        value="00:00"
                    >

                </div>


                <div class="age-group full">

                    <button
                        class="age-button"
                        onclick="calculateAge()">

                        🎂 Find Exact Age

                    </button>

                </div>

            </div>


            <div
                class="age-result"
                id="ageResult">

                <div class="age-main">

                    <h3>
                        Enter Your Birthday
                    </h3>

                    <p>
                        Your exact age will appear here.
                    </p>

                </div>

            </div>

        </div>

    `;
}


/* =========================================================
   CALCULATE AGE
========================================================= */

function calculateAge(){

    const dateValue=
        document.getElementById("dob").value;

    const timeValue=
        document.getElementById("birthTime").value;

    if(!dateValue){

        alert(
            "Please select your date of birth."
        );

        return;
    }

    birthDate=
        new Date(
            dateValue+
            "T"+
            (timeValue||"00:00")
        );

    if(isNaN(birthDate.getTime())){

        alert(
            "Please enter a valid date and time."
        );

        return;
    }

    if(birthDate>new Date()){

        alert(
            "Birth date cannot be in the future."
        );

        return;
    }

    clearAgeTimer();

    updateAge();

    ageTimer=
        setInterval(
            updateAge,
            1000
        );
}


/* =========================================================
   UPDATE AGE
========================================================= */

function updateAge(){

    if(!birthDate){
        return;
    }

    const now=new Date();

    let years=
        now.getFullYear()-
        birthDate.getFullYear();

    let birthdayThisYear=
        new Date(
            now.getFullYear(),
            birthDate.getMonth(),
            birthDate.getDate(),
            birthDate.getHours(),
            birthDate.getMinutes(),
            birthDate.getSeconds()
        );

    if(now<birthdayThisYear){
        years--;
    }

    let lastBirthday=
        new Date(
            birthDate.getFullYear()+years,
            birthDate.getMonth(),
            birthDate.getDate(),
            birthDate.getHours(),
            birthDate.getMinutes(),
            birthDate.getSeconds()
        );

    let difference=
        now.getTime()-
        lastBirthday.getTime();

    let totalSeconds=
        Math.floor(
            difference/1000
        );

    let days=
        Math.floor(
            totalSeconds/86400
        );

    totalSeconds%=86400;

    let hours=
        Math.floor(
            totalSeconds/3600
        );

    totalSeconds%=3600;

    let minutes=
        Math.floor(
            totalSeconds/60
        );

    let seconds=
        totalSeconds%60;


    let nextBirthday=
        new Date(
            now.getFullYear(),
            birthDate.getMonth(),
            birthDate.getDate(),
            birthDate.getHours(),
            birthDate.getMinutes(),
            birthDate.getSeconds()
        );

    if(nextBirthday<=now){

        nextBirthday=
            new Date(
                now.getFullYear()+1,
                birthDate.getMonth(),
                birthDate.getDate(),
                birthDate.getHours(),
                birthDate.getMinutes(),
                birthDate.getSeconds()
            );
    }

    let birthdayDifference=
        nextBirthday.getTime()-
        now.getTime();

    let birthdayDays=
        Math.floor(
            birthdayDifference/86400000
        );

    let birthdayHours=
        Math.floor(
            (birthdayDifference%86400000)/
            3600000
        );

    let birthdayMinutes=
        Math.floor(
            (birthdayDifference%3600000)/
            60000
        );

    let birthdaySeconds=
        Math.floor(
            (birthdayDifference%60000)/
            1000
        );


    document.getElementById("ageResult").innerHTML=`

        <div class="age-main">

            <h3>
                ${years} Years Old
            </h3>

            <p>
                ${days} days,
                ${hours} hours,
                ${minutes} minutes,
                ${seconds} seconds
            </p>

        </div>


        <div class="age-grid">

            <div class="age-box">
                <strong>${years}</strong>
                Years
            </div>

            <div class="age-box">
                <strong>${days}</strong>
                Days
            </div>

            <div class="age-box">
                <strong>${hours}</strong>
                Hours
            </div>

            <div class="age-box">
                <strong>${minutes}</strong>
                Minutes
            </div>

        </div>


        <div class="birthday-box">

            🎉 NEXT BIRTHDAY

            <br><br>

            <strong>

                ${birthdayDays} days
                ${birthdayHours} hours
                ${birthdayMinutes} minutes
                ${birthdaySeconds} seconds

            </strong>

        </div>

    `;
}

function clearAgeTimer(){

    if(ageTimer){

        clearInterval(ageTimer);

        ageTimer=null;
    }
}


/* =========================================================
   OPEN CURRENT
========================================================= */

function openCurrent(){

    if(currentURL!==""){

        window.open(
            currentURL,
            "_blank",
            "noopener,noreferrer"
        );
    }
}


/* =========================================================
   NOVACV SKILL DATABASE
========================================================= */

const SKILL_BANK={

    "Python":["python"],
    "Java":["java"],
    "JavaScript":["javascript","js"],
    "React":["react","reactjs"],
    "Node.js":["node.js","nodejs"],
    "Django":["django"],
    "Flask":["flask"],
    "SQL":["sql","mysql","postgresql"],
    "MongoDB":["mongodb"],
    "Git":["git","github"],
    "HTML":["html"],
    "CSS":["css"],
    "Bootstrap":["bootstrap"],
    "REST APIs":["rest api","restful","api"],
    "Machine Learning":["machine learning","ml"],
    "Data Analysis":["data analysis","data analytics"],
    "Power BI":["power bi"],
    "Excel":["excel","ms excel"],
    "Tableau":["tableau"],
    "C":["c programming"],
    "C++":["c++"],
    "AWS":["aws"],
    "Azure":["azure"],
    "Docker":["docker"],
    "Linux":["linux"],
    "UI/UX":["ui/ux","figma"],
    "Communication":["communication"],
    "Leadership":["leadership"],
    "Problem Solving":["problem solving"]

};


const JOB_PROFILES=[

    {
        title:"Junior Python Developer",
        company:"TechCore Labs",
        skills:[
            "Python",
            "Django",
            "SQL",
            "Git",
            "REST APIs"
        ],
        level:"Entry level"
    },

    {
        title:"Data Analyst",
        company:"InsightWorks",
        skills:[
            "Python",
            "SQL",
            "Excel",
            "Power BI",
            "Data Analysis"
        ],
        level:"Entry level"
    },

    {
        title:"Frontend Developer",
        company:"PixelForge",
        skills:[
            "HTML",
            "CSS",
            "JavaScript",
            "React",
            "Git"
        ],
        level:"Entry level"
    },

    {
        title:"Full Stack Developer",
        company:"CloudSprint",
        skills:[
            "HTML",
            "CSS",
            "JavaScript",
            "React",
            "Node.js",
            "SQL",
            "Git",
            "REST APIs"
        ],
        level:"Entry level"
    },

    {
        title:"ML Intern / Trainee",
        company:"NextMind AI",
        skills:[
            "Python",
            "Machine Learning",
            "SQL",
            "Data Analysis"
        ],
        level:"Internship"
    }

];


/* =========================================================
   DEMO RESUME
========================================================= */

const demoResume=`

ARUN KUMAR

Email: arun.kumar@email.com
Phone: +91 98765 43210
LinkedIn: linkedin.com/in/arun-kumar

PROFESSIONAL SUMMARY

B.Sc Computer Science graduate with strong interest in
software development and data analytics. Built web
applications using Python, Django, JavaScript and SQL.

EDUCATION

B.Sc Computer Science - ABC College - 2026

TECHNICAL SKILLS

Python, Django, JavaScript, HTML, CSS, Bootstrap,
SQL, MySQL, Git, GitHub, REST APIs, Excel, Power BI

PROJECTS

Student Management System

Developed a Django and MySQL web application for
student records and authentication.

Inventory Dashboard

Built a responsive dashboard with JavaScript, SQL
and Power BI concepts to analyze 1,500+ records.

INTERNSHIP

Software Development Intern

Built REST API modules, improved data processing
workflow and tested application features.

CERTIFICATIONS

Python Programming Certificate

ACHIEVEMENTS

Automated a weekly reporting workflow and reduced
manual work by 30%.

Led a 4-member college project team and delivered
the project before deadline.

`;


/* =========================================================
   SHOW NOVACV
========================================================= */

function showResumeAnalyzer(){

    clearAgeTimer();

    currentURL="";

    document.getElementById("pageTitle").innerText=
        "NovaCV AI Resume Analyzer";

    document.getElementById("openButton").innerText=
        "Top";

    document.getElementById("displayArea").innerHTML=`

        <div class="cv-page">

            <section class="cv-hero">

                <div class="eyebrow">
                    AI CAREER INTELLIGENCE PLATFORM
                </div>

                <h1>
                    Turn your resume into a
                    <span>career strategy.</span>
                </h1>

                <p>
                    Analyze ATS readiness, discover skill gaps,
                    understand job matching and create a practical
                    improvement plan.
                </p>

                <div class="hero-stats">

                    <span>⚡ Instant Analysis</span>
                    <span>🎯 Role Matching</span>
                    <span>📈 Skill Gap Roadmap</span>

                </div>

            </section>


            <section class="cv-workspace">

                <div class="cv-panel">

                    <div class="panel-head">

                        <div>

                            <div class="kicker">
                                STEP 01
                            </div>

                            <h2>
                                Upload your resume
                            </h2>

                        </div>

                        <span class="secure">
                            🔒 Private by design
                        </span>

                    </div>


                    <label
                        class="dropzone"
                        for="resumeFile"
                        id="dropzone">

                        <div class="upload-icon">
                            ↑
                        </div>

                        <strong>
                            Drop your resume here
                        </strong>

                        <small>
                            PDF / DOCX / TXT · up to 8 MB
                        </small>

                        <em>
                            or click to browse
                        </em>

                        <input
                            id="resumeFile"
                            type="file"
                            accept=".pdf,.docx,.txt"
                            hidden
                        >

                    </label>


                    <div
                        class="file-row"
                        id="fileRow"
                        hidden>

                        <span id="fileName">
                            No file
                        </span>

                        <button
                            class="mini"
                            onclick="clearFile(event)">

                            Remove

                        </button>

                    </div>


                    <div class="or">
                        <span>OR</span>
                    </div>


                    <textarea
                        id="resumeText"
                        placeholder="Paste resume text here for the fastest demo..."></textarea>


                    <div class="actions">

                        <button
                            class="primary"
                            onclick="analyzeResume()">

                            Analyze Resume →

                        </button>

                        <button
                            class="secondary"
                            onclick="clearResume()">

                            Clear

                        </button>

                    </div>


                    <div
                        id="status"
                        class="status">
                    </div>

                </div>


                <div class="cv-panel score-panel">

                    <div class="kicker">
                        AI READINESS
                    </div>

                    <h2>
                        Your career health
                    </h2>


                    <div class="score-wrap">

                        <div
                            class="ring"
                            id="scoreRing">

                            <div>

                                <strong id="score">
                                    —
                                </strong>

                                <span>
                                    /100
                                </span>

                            </div>

                        </div>


                        <div>

                            <div
                                class="score-label"
                                id="scoreLabel">

                                Waiting for analysis

                            </div>

                            <p id="scoreText">

                                Upload a resume to generate
                                your personalized report.

                            </p>

                        </div>

                    </div>


                    <div class="mini-grid">

                        <div>
                            <b id="skillCount">—</b>
                            <span>Skills found</span>
                        </div>

                        <div>
                            <b id="wordCount">—</b>
                            <span>Words</span>
                        </div>

                        <div>
                            <b id="metricCount">—</b>
                            <span>Metrics</span>
                        </div>

                    </div>

                </div>

            </section>


            <section class="cv-insights">

                <div class="cv-panel">

                    <div class="panel-head">

                        <div>

                            <div class="kicker">
                                STEP 02
                            </div>

                            <h2>
                                Skill intelligence
                            </h2>

                        </div>

                        <span
                            class="pill"
                            id="skillPill">

                            0 detected

                        </span>

                    </div>


                    <div
                        id="skills"
                        class="chips">

                        <div class="empty">
                            Your detected skills will appear here.
                        </div>

                    </div>

                </div>


                <div class="cv-panel">

                    <div class="panel-head">

                        <div>

                            <div class="kicker">
                                STEP 03
                            </div>

                            <h2>
                                Skill-gap radar
                            </h2>

                        </div>

                        <span class="pill warn">
                            Improve strategically
                        </span>

                    </div>


                    <div
                        id="gaps"
                        class="gap-list">

                        <div class="empty">
                            Analyze a resume to see your priority
                            skill gaps.
                        </div>

                    </div>

                </div>

            </section>


            <section class="cv-insights">

                <div class="cv-panel">

                    <div class="panel-head">

                        <div>

                            <div class="kicker">
                                SIGNAL CHECK
                            </div>

                            <h2>
                                Resume strengths
                            </h2>

                        </div>

                    </div>


                    <div
                        id="strengths"
                        class="list">

                        <div class="empty">
                            —
                        </div>

                    </div>

                </div>


                <div class="cv-panel">

                    <div class="panel-head">

                        <div>

                            <div class="kicker">
                                NEXT ACTIONS
                            </div>

                            <h2>
                                Improvement plan
                            </h2>

                        </div>

                    </div>


                    <div
                        id="suggestions"
                        class="list numbered">

                        <div class="empty">
                            —
                        </div>

                    </div>

                </div>

            </section>


            <section class="cv-panel cv-jobs">

                <div class="panel-head">

                    <div>

                        <div class="kicker">
                            STEP 04
                        </div>

                        <h2>
                            Career match engine
                        </h2>

                        <p class="muted">
                            Illustrative role matching based on
                            skills detected from your resume.
                        </p>

                    </div>

                    <button
                        class="secondary"
                        onclick="downloadReport()">

                        Download Report

                    </button>

                </div>


                <div
                    id="jobsGrid"
                    class="jobs-grid">

                    <div class="empty">
                        Your matched roles will appear
                        after analysis.
                    </div>

                </div>

            </section>


            <section class="cv-how">

                <div>

                    <div class="kicker">
                        HOW IT WORKS
                    </div>

                    <h2>
                        One resume. Four layers of intelligence.
                    </h2>

                </div>


                <div class="steps">

                    <div>
                        <b>01</b>
                        <h3>Parse</h3>
                        <p>
                            Extract role signals, skills,
                            sections and evidence.
                        </p>
                    </div>

                    <div>
                        <b>02</b>
                        <h3>Score</h3>
                        <p>
                            Measure ATS structure,
                            completeness and impact.
                        </p>
                    </div>

                    <div>
                        <b>03</b>
                        <h3>Match</h3>
                        <p>
                            Compare your profile with
                            target career paths.
                        </p>
                    </div>

                    <div>
                        <b>04</b>
                        <h3>Improve</h3>
                        <p>
                            Get concrete actions instead
                            of generic advice.
                        </p>
                    </div>

                </div>

            </section>

        </div>

    `;

    setupResumeUpload();
}


/* =========================================================
   RESUME UPLOAD
========================================================= */

function setupResumeUpload(){

    const dz=
        document.getElementById("dropzone");

    const input=
        document.getElementById("resumeFile");

    if(!dz||!input){
        return;
    }

    ["dragenter","dragover"].forEach(
        eventName=>{

            dz.addEventListener(
                eventName,
                event=>{

                    event.preventDefault();

                    dz.classList.add("drag");

                }
            );

        }
    );


    ["dragleave","drop"].forEach(
        eventName=>{

            dz.addEventListener(
                eventName,
                event=>{

                    event.preventDefault();

                    dz.classList.remove("drag");

                }
            );

        }
    );


    dz.addEventListener(
        "drop",
        event=>{

            handleResumeFile(
                event.dataTransfer.files[0]
            );

        }
    );


    input.addEventListener(
        "change",
        event=>{

            handleResumeFile(
                event.target.files[0]
            );

        }
    );
}


/* =========================================================
   HANDLE FILE
========================================================= */

function handleResumeFile(file){

    if(!file){
        return;
    }

    selectedFile=file;

    const fileRow=
        document.getElementById("fileRow");

    const fileName=
        document.getElementById("fileName");

    const status=
        document.getElementById("status");

    fileName.textContent=
        `${file.name} · ${(file.size/1024).toFixed(0)} KB`;

    fileRow.hidden=false;

    const ext=
        file.name
        .split(".")
        .pop()
        .toLowerCase();


    if(ext==="txt"){

        file.text().then(
            text=>{

                document.getElementById(
                    "resumeText"
                ).value=text;

                status.textContent=
                    "TXT file loaded. Click Analyze Resume.";

            }
        );

    }else{

        status.textContent=
            "For browser-only mode, paste PDF/DOCX text into the box below.";
    }
}


/* =========================================================
   CLEAR FILE
========================================================= */

function clearFile(event){

    event.preventDefault();

    selectedFile=null;

    const input=
        document.getElementById("resumeFile");

    if(input){
        input.value="";
    }

    const fileRow=
        document.getElementById("fileRow");

    if(fileRow){
        fileRow.hidden=true;
    }
}


/* =========================================================
   DEMO RESUME
========================================================= */

function loadDemoResume(){

    document.getElementById(
        "resumeText"
    ).value=demoResume;

    document.getElementById(
        "status"
    ).textContent=
        "Demo resume loaded.";

}


/* =========================================================
   NORMALIZE
========================================================= */

function normalizeText(text){

    return text
        .toLowerCase()
        .replace(/\n/g," ")
        .replace(/\s+/g," ");
}


/* =========================================================
   EXTRACT SKILLS
========================================================= */

function extractSkills(text){

    const t=
        normalizeText(text);

    const found=[];

    for(
        const [skill,aliases]
        of Object.entries(SKILL_BANK)
    ){

        if(
            aliases.some(
                alias=>t.includes(alias.toLowerCase())
            )
        ){

            found.push(skill);

        }

    }

    return[
        ...new Set(found)
    ].sort();

}


/* =========================================================
   ANALYZE RESUME DATA
========================================================= */

function analyzeResumeData(text){

    const t=
        normalizeText(text);

    const skills=
        extractSkills(text);


    const sections={

        "Contact information":
            /email|phone|mobile|linkedin/.test(t),

        "Professional summary":
            /professional summary|profile|objective|summary/.test(t),

        "Education":
            /education|degree|bachelor|master|b\.sc|btech|bba|bcom|mca/.test(t),

        "Experience":
            /experience|internship|work history|employment/.test(t),

        "Projects":
            /projects|project experience/.test(t),

        "Skills":
            /\bskills\b|technical skills|technologies/.test(t),

        "Certifications":
            /certification|certifications|certificate/.test(t)

    };


    const sectionPoints=
        Object.values(sections)
        .filter(Boolean)
        .length*8;


    const words=
        text
        .trim()
        .split(/\s+/)
        .filter(Boolean)
        .length;


    const lengthPoints=
        words>=250&&words<=900
        ?10
        :4;


    const actionWords=
        (
            t.match(
                /\b(led|built|developed|designed|implemented|optimized|automated|created|improved|analyzed|managed)\b/g
            )||[]
        ).length;


    const impactPoints=
        actionWords>=5
        ?8
        :3;


    const metrics=
        (
            t.match(
                /\b\d+%|\b\d+\+|\b\d+x|\b\d+ (users|projects|clients|records|hours|days)\b/g
            )||[]
        ).length;


    const metricsPoints=
        metrics>=2
        ?8
        :2;


    const keywords=[
        "resume",
        "experience",
        "education",
        "skills",
        "project",
        "linkedin",
        "email",
        "phone"
    ];


    const keywordPoints=
        Math.min(
            16,
            keywords.filter(
                keyword=>t.includes(keyword)
            ).length*2
        );


    const score=
        Math.min(
            100,
            sectionPoints+
            lengthPoints+
            impactPoints+
            metricsPoints+
            keywordPoints
        );


    const target=
        new Set(
            JOB_PROFILES.flatMap(
                job=>job.skills
            )
        );


    const gaps=
        [...target]
        .filter(
            skill=>!skills.includes(skill)
        )
        .sort()
        .slice(0,12);


    const strengths=[];


    if(skills.length>=8){
        strengths.push(
            "Strong technical skill coverage"
        );
    }

    if(sections.Projects){
        strengths.push(
            "Projects section detected"
        );
    }

    if(actionWords>=5){
        strengths.push(
            "Good use of action-oriented verbs"
        );
    }

    if(metrics>=2){
        strengths.push(
            "Includes measurable achievements"
        );
    }

    if(!strengths.length){

        strengths.push(
            "Good base profile — add more evidence and keywords"
        );

    }


    const suggestions=[];


    if(!sections["Professional summary"]){

        suggestions.push(
            "Add a 2–3 line professional summary tailored to the target role."
        );

    }


    if(!sections.Projects){

        suggestions.push(
            "Add 2–3 projects with technology, action and measurable outcome."
        );

    }


    if(metrics<2){

        suggestions.push(
            "Quantify achievements: time saved, users served, revenue, accuracy, marks, or volume."
        );

    }


    if(skills.length<6){

        suggestions.push(
            "Expand the technical skills section with role-relevant tools used in real projects."
        );

    }


    if(!sections.Certifications){

        suggestions.push(
            "Add relevant certifications or training with completion dates."
        );

    }


    suggestions.push(
        "Mirror important keywords from the job description naturally; avoid keyword stuffing."
    );


    const jobs=
        JOB_PROFILES
        .map(job=>{

            const overlap=
                job.skills.filter(
                    skill=>skills.includes(skill)
                ).length;

            return{

                ...job,

                match:
                    Math.round(
                        35+
                        (
                            overlap/
                            Math.max(
                                1,
                                job.skills.length
                            )
                        )*65
                    ),

                missing:
                    job.skills.filter(
                        skill=>!skills.includes(skill)
                    )

            };

        })
        .sort(
            (a,b)=>b.match-a.match
        );


    return{

        score,
        skills,
        skill_count:skills.length,
        sections,
        strengths,
        gaps,
        suggestions,
        jobs,
        word_count:words,
        metrics

    };

}


/* =========================================================
   ANALYZE BUTTON
========================================================= */

function analyzeResume(){

    const text=
        document
        .getElementById("resumeText")
        .value
        .trim();

    const status=
        document.getElementById("status");


    if(!text){

        status.textContent=
            "Please paste your resume text first.";

        return;
    }


    status.textContent=
        "Analyzing resume intelligence…";


    setTimeout(
        ()=>{

            lastResult=
                analyzeResumeData(text);

            renderResume(lastResult);

            status.textContent=
                "Analysis complete. Your dashboard is ready.";

        },
        500
    );

}


/* =========================================================
   RENDER RESUME
========================================================= */

function renderResume(r){

    setScore(r.score);


    document.getElementById(
        "skillPill"
    ).textContent=
        `${r.skill_count} detected`;


    const skills=
        document.getElementById("skills");

    skills.innerHTML=
        r.skills.length
        ?

        r.skills
        .map(
            skill=>
                `<span class="chip">
                    ${escapeHtml(skill)}
                </span>`
        )
        .join("")

        :

        `<div class="empty">
            No recognizable skills detected.
        </div>`;


    const gaps=
        document.getElementById("gaps");

    gaps.innerHTML=
        r.gaps.length

        ?

        r.gaps
        .map(
            gap=>
                `<div class="gap">

                    <b>
                        ${escapeHtml(gap)}
                    </b>

                    <span>
                        Priority gap
                    </span>

                </div>`
        )
        .join("")

        :

        `<div class="empty">
            No major gaps found.
        </div>`;


    document.getElementById(
        "strengths"
    ).innerHTML=
        r.strengths
        .map(
            strength=>
                `<div class="list-item">

                    <span class="dot"></span>

                    <span>
                        ${escapeHtml(strength)}
                    </span>

                </div>`
        )
        .join("");


    document.getElementById(
        "suggestions"
    ).innerHTML=
        r.suggestions
        .map(
            (suggestion,index)=>
                `<div class="list-item">

                    <span class="num">
                        ${index+1}
                    </span>

                    <span>
                        ${escapeHtml(suggestion)}
                    </span>

                </div>`
        )
        .join("");


    document.getElementById(
        "jobsGrid"
    ).innerHTML=
        r.jobs
        .map(
            job=>
                `<div class="job">

                    <div class="job-top">

                        <div>

                            <h3>
                                ${escapeHtml(job.title)}
                            </h3>

                            <small>
                                ${escapeHtml(job.company)}
                                ·
                                ${escapeHtml(job.level)}
                            </small>

                        </div>

                        <div class="match">
                            ${job.match}%
                        </div>

                    </div>


                    <div class="bar">

                        <i
                            style="width:${job.match}%">
                        </i>

                    </div>


                    <div class="missing">

                        ${
                            job.missing.length

                            ?

                            `Missing:
                            ${job.missing
                                .map(escapeHtml)
                                .join(", ")}`

                            :

                            "No major missing skills"
                        }

                    </div>

                </div>`
        )
        .join("");

}


/* =========================================================
   SCORE
========================================================= */

function setScore(n){

    document.getElementById(
        "score"
    ).textContent=
        n??"—";


    const ring=
        document.getElementById("scoreRing");


    const deg=
        n
        ?Math.round(n*3.6)
        :0;


    ring.style.background=
        `conic-gradient(
            #8c72ff 0deg ${deg}deg,
            #1a2940 ${deg}deg 360deg
        )`;


    document.getElementById(
        "skillCount"
    ).textContent=
        lastResult?.skill_count??"—";


    document.getElementById(
        "wordCount"
    ).textContent=
        lastResult?.word_count??"—";


    document.getElementById(
        "metricCount"
    ).textContent=
        lastResult?.metrics??"—";


    document.getElementById(
        "scoreLabel"
    ).textContent=

        n

        ?

        (
            n>=85
            ?"Excellent ATS foundation"
            :
            n>=70
            ?"Strong foundation"
            :
            n>=55
            ?"Needs targeted improvements"
            :
            "Major improvement opportunities"
        )

        :

        "Waiting for analysis";


    document.getElementById(
        "scoreText"
    ).textContent=

        n

        ?

        `Your profile scored ${n}/100 across
        structure, relevance signals and evidence.`

        :

        "Upload a resume to generate your personalized report.";

}


/* =========================================================
   CLEAR RESUME
========================================================= */

function clearResume(){

    lastResult=null;

    const text=
        document.getElementById("resumeText");

    if(text){
        text.value="";
    }

    const status=
        document.getElementById("status");

    if(status){
        status.textContent="";
    }

    document.getElementById(
        "skills"
    ).innerHTML=
        `<div class="empty">
            Your detected skills will appear here.
        </div>`;


    document.getElementById(
        "gaps"
    ).innerHTML=
        `<div class="empty">
            Analyze a resume to see your priority skill gaps.
        </div>`;


    document.getElementById(
        "strengths"
    ).innerHTML=
        `<div class="empty">—</div>`;


    document.getElementById(
        "suggestions"
    ).innerHTML=
        `<div class="empty">—</div>`;


    document.getElementById(
        "jobsGrid"
    ).innerHTML=
        `<div class="empty">
            Your matched roles will appear after analysis.
        </div>`;


    setScore(null);

}


/* =========================================================
   DOWNLOAD REPORT
========================================================= */

function downloadReport(){

    if(!lastResult){

        document.getElementById(
            "status"
        ).textContent=
            "Analyze a resume first.";

        return;
    }


    const payload={

        product:"NovaCV AI",

        generated_at:
            new Date().toISOString(),

        analysis:lastResult

    };


    const blob=
        new Blob(
            [
                JSON.stringify(
                    payload,
                    null,
                    2
                )
            ],
            {
                type:"application/json"
            }
        );


    const url=
        URL.createObjectURL(blob);


    const a=
        document.createElement("a");


    a.href=url;

    a.download=
        "novacv-ai-report.json";


    document.body.appendChild(a);

    a.click();

    a.remove();


    setTimeout(
        ()=>URL.revokeObjectURL(url),
        500
    );

}


/* =========================================================
   ESCAPE HTML
========================================================= */

function escapeHtml(value){

    return String(value)
        .replace(
            /[&<>'"]/g,
            char=>({

                "&":"&amp;",
                "<":"&lt;",
                ">":"&gt;",
                "'":"&#39;",
                '"':"&quot;"

            }[char])
        );

}

</script>

</body>
</html>
```
