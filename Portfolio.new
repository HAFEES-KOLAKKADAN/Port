<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Hafees Ali K | 3D Portfolio</title>

<style>

/* ==============================
   RESET
================================ */

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    scroll-behavior:smooth;
}

html{
    scroll-behavior:smooth;
}

body{
    font-family:Arial, Helvetica, sans-serif;
    background:#02040a;
    color:white;
    overflow-x:hidden;
}

a{
    text-decoration:none;
    color:inherit;
}


/* ==============================
   3D BACKGROUND
================================ */

#canvas{
    position:fixed;
    top:0;
    left:0;
    width:100%;
    height:100%;
    z-index:-10;
}

body::before{
    content:"";
    position:fixed;
    width:500px;
    height:500px;
    background:#00eaff;
    border-radius:50%;
    filter:blur(180px);
    opacity:.12;
    top:-200px;
    left:-200px;
    z-index:-5;
}

body::after{
    content:"";
    position:fixed;
    width:500px;
    height:500px;
    background:#7b2cff;
    border-radius:50%;
    filter:blur(180px);
    opacity:.13;
    right:-200px;
    bottom:-200px;
    z-index:-5;
}


/* ==============================
   NAVIGATION
================================ */

nav{
    position:fixed;
    top:0;
    left:0;
    width:100%;
    height:75px;

    display:flex;
    justify-content:space-between;
    align-items:center;

    padding:0 8%;

    background:rgba(2,4,10,.55);
    backdrop-filter:blur(20px);

    border-bottom:1px solid rgba(255,255,255,.08);

    z-index:1000;
}

.logo{
    font-size:25px;
    font-weight:bold;
    letter-spacing:3px;
    color:#00eaff;

    text-shadow:
        0 0 10px #00eaff,
        0 0 30px #00eaff;
}

nav ul{
    display:flex;
    gap:30px;
    list-style:none;
}

nav ul li a{
    color:#aaa;
    font-size:14px;
    transition:.3s;
}

nav ul li a:hover{
    color:#00eaff;
    text-shadow:0 0 10px #00eaff;
}


/* ==============================
   HERO
================================ */

.hero{
    min-height:100vh;

    display:flex;
    justify-content:center;
    align-items:center;

    padding:120px 20px 80px;

    text-align:center;

    perspective:1000px;
}

.hero-content{
    max-width:900px;

    transform-style:preserve-3d;

    transition:transform .2s ease;
}


/* ==============================
   PROFILE
================================ */

.profile-container{
    width:210px;
    height:210px;

    margin:0 auto 35px;

    position:relative;

    transform-style:preserve-3d;

    animation:profileFloat 4s ease-in-out infinite;
}

.profile-container::before{
    content:"";

    position:absolute;

    inset:-15px;

    border-radius:50%;

    border:1px solid #00eaff;

    box-shadow:
        0 0 20px #00eaff,
        inset 0 0 20px #00eaff;

    animation:rotateRing 8s linear infinite;
}

.profile-container::after{
    content:"";

    position:absolute;

    inset:-30px;

    border-radius:50%;

    border:1px solid rgba(123,44,255,.7);

    animation:rotateRingReverse 12s linear infinite;
}

.profile{
    width:190px;
    height:190px;

    object-fit:cover;

    border-radius:50%;

    border:4px solid #00eaff;

    padding:5px;

    background:#02040a;

    box-shadow:
        0 0 20px #00eaff,
        0 0 60px rgba(0,234,255,.5);

    position:relative;

    z-index:5;
}

.status{
    position:absolute;

    right:15px;
    bottom:20px;

    width:22px;
    height:22px;

    border-radius:50%;

    background:#00ff88;

    border:4px solid #02040a;

    box-shadow:0 0 20px #00ff88;

    z-index:10;
}

@keyframes profileFloat{

    0%,100%{
        transform:translateY(0) rotateY(0deg);
    }

    50%{
        transform:translateY(-15px) rotateY(10deg);
    }
}

@keyframes rotateRing{

    from{
        transform:rotateZ(0deg);
    }

    to{
        transform:rotateZ(360deg);
    }
}

@keyframes rotateRingReverse{

    from{
        transform:rotateZ(360deg);
    }

    to{
        transform:rotateZ(0deg);
    }
}


/* ==============================
   HERO TEXT
================================ */

.hero h1{
    font-size:clamp(45px,8vw,90px);

    font-weight:900;

    letter-spacing:5px;

    margin-bottom:15px;

    background:
        linear-gradient(
            90deg,
            #ffffff,
            #00eaff,
            #7b2cff,
            #00eaff,
            #ffffff
        );

    background-size:400%;

    -webkit-background-clip:text;
    color:transparent;

    animation:gradientMove 7s linear infinite;

    text-shadow:
        0 0 30px rgba(0,234,255,.2);
}

@keyframes gradientMove{

    0%{
        background-position:0%;
    }

    100%{
        background-position:400%;
    }
}

.hero h2{
    color:#00eaff;

    font-size:20px;

    margin-bottom:25px;

    letter-spacing:2px;
}

.typing{
    color:#aaa;

    font-size:17px;

    min-height:30px;
}

.cursor{
    color:#00eaff;
    animation:blink .7s infinite;
}

@keyframes blink{

    0%,50%{
        opacity:1;
    }

    51%,100%{
        opacity:0;
    }
}


/* ==============================
   BUTTONS
================================ */

.buttons{
    margin-top:35px;

    display:flex;

    justify-content:center;

    gap:18px;

    flex-wrap:wrap;
}

.btn{
    position:relative;

    padding:15px 30px;

    border:1px solid #00eaff;

    border-radius:50px;

    color:#00eaff;

    overflow:hidden;

    transition:.4s;

    background:rgba(0,234,255,.03);
}

.btn::before{
    content:"";

    position:absolute;

    left:-100%;

    top:0;

    width:100%;
    height:100%;

    background:#00eaff;

    transition:.4s;

    z-index:-1;
}

.btn:hover::before{
    left:0;
}

.btn:hover{
    color:#000;

    box-shadow:
        0 0 20px #00eaff,
        0 0 50px rgba(0,234,255,.4);

    transform:translateY(-5px) translateZ(20px);
}

.btn.purple{
    border-color:#7b2cff;
    color:#c59cff;
}

.btn.purple::before{
    background:#7b2cff;
}

.btn.purple:hover{
    color:white;

    box-shadow:
        0 0 20px #7b2cff;
}


/* ==============================
   SECTIONS
================================ */

section{
    padding:120px 8%;
}

.title{
    text-align:center;

    font-size:45px;

    margin-bottom:60px;
}

.title span{
    color:#00eaff;

    text-shadow:
        0 0 20px #00eaff;
}


/* ==============================
   ABOUT
================================ */

.about-box{
    max-width:900px;

    margin:auto;

    padding:45px;

    background:
        linear-gradient(
            145deg,
            rgba(0,234,255,.08),
            rgba(123,44,255,.06)
        );

    border:1px solid rgba(0,234,255,.2);

    border-radius:25px;

    text-align:center;

    line-height:1.9;

    color:#aaa;

    transform-style:preserve-3d;

    transition:.4s;
}

.about-box:hover{
    transform:
        perspective(1000px)
        rotateX(3deg)
        rotateY(-3deg)
        translateY(-8px);

    box-shadow:
        0 20px 60px rgba(0,234,255,.1);
}

.about-box strong{
    color:#00eaff;
}


/* ==============================
   SKILLS
================================ */

.skills{
    max-width:1100px;

    margin:auto;

    display:grid;

    grid-template-columns:
        repeat(auto-fit,minmax(180px,1fr));

    gap:25px;

    perspective:1000px;
}

.skill-card{
    padding:35px 20px;

    text-align:center;

    background:
        linear-gradient(
            145deg,
            rgba(255,255,255,.04),
            rgba(0,234,255,.02)
        );

    border:1px solid rgba(255,255,255,.1);

    border-radius:20px;

    transition:.4s;

    transform-style:preserve-3d;
}

.skill-card:hover{
    transform:
        rotateX(8deg)
        rotateY(-8deg)
        translateY(-12px);

    border-color:#00eaff;

    box-shadow:
        0 20px 50px rgba(0,234,255,.15);
}

.skill-icon{
    font-size:45px;

    margin-bottom:15px;

    filter:
        drop-shadow(0 0 10px #00eaff);
}

.skill-card h3{
    margin-bottom:10px;
}

.skill-card p{
    color:#777;
    font-size:13px;
}


/* ==============================
   PROJECTS
================================ */

.projects{
    max-width:1100px;

    margin:auto;

    display:grid;

    grid-template-columns:
        repeat(auto-fit,minmax(280px,1fr));

    gap:30px;

    perspective:1000px;
}

.project{
    padding:35px;

    min-height:260px;

    border-radius:22px;

    background:
        linear-gradient(
            145deg,
            rgba(0,234,255,.08),
            rgba(123,44,255,.06)
        );

    border:1px solid rgba(255,255,255,.1);

    transition:.4s;

    transform-style:preserve-3d;
}

.project:hover{
    transform:
        rotateX(5deg)
        rotateY(-5deg)
        translateY(-15px)
        translateZ(20px);

    border-color:#00eaff;

    box-shadow:
        0 25px 70px rgba(0,234,255,.15);
}

.project-number{
    color:#00eaff;

    font-size:14px;

    letter-spacing:3px;

    margin-bottom:20px;
}

.project h3{
    font-size:23px;

    margin-bottom:15px;
}

.project p{
    color:#888;

    line-height:1.7;

    margin-bottom:25px;
}

.project-link{
    color:#00eaff;

    font-size:14px;
}


/* ==============================
   EDUCATION
================================ */

.timeline{
    max-width:800px;

    margin:auto;

    border-left:2px solid #00eaff;

    padding-left:35px;
}

.timeline-item{
    position:relative;

    margin-bottom:50px;

    padding:25px;

    border-radius:18px;

    background:rgba(255,255,255,.03);

    border:1px solid rgba(255,255,255,.08);

    transition:.3s;
}

.timeline-item:hover{
    border-color:#00eaff;

    transform:translateX(10px);

    box-shadow:
        0 0 30px rgba(0,234,255,.1);
}

.timeline-item::before{
    content:"";

    position:absolute;

    width:18px;
    height:18px;

    border-radius:50%;

    background:#00eaff;

    box-shadow:0 0 20px #00eaff;

    left:-45px;

    top:30px;
}

.timeline-item h3{
    color:#00eaff;

    margin-bottom:10px;
}

.timeline-item p{
    color:#888;

    line-height:1.7;
}


/* ==============================
   CONTACT
================================ */

.contact{
    text-align:center;

    max-width:700px;

    margin:auto;
}

.contact p{
    color:#888;

    line-height:1.8;

    margin-bottom:30px;
}

.socials{
    display:flex;

    justify-content:center;

    flex-wrap:wrap;

    gap:15px;
}

.social{
    padding:13px 25px;

    border:1px solid #333;

    border-radius:30px;

    transition:.3s;
}

.social:hover{
    color:#00eaff;

    border-color:#00eaff;

    box-shadow:
        0 0 20px rgba(0,234,255,.2);

    transform:translateY(-5px);
}


/* ==============================
   FOOTER
================================ */

footer{
    text-align:center;

    padding:30px;

    color:#555;

    border-top:1px solid rgba(255,255,255,.08);

    font-size:13px;
}

footer span{
    color:#00eaff;
}


/* ==============================
   SCROLL INDICATOR
================================ */

.scroll{
    position:absolute;

    bottom:25px;

    left:50%;

    transform:translateX(-50%);

    color:#555;

    font-size:12px;

    letter-spacing:3px;
}


/* ==============================
   MOBILE
================================ */

@media(max-width:700px){

    nav{
        padding:0 5%;
    }

    nav ul{
        display:none;
    }

    section{
        padding:90px 6%;
    }

    .hero h1{
        font-size:48px;
        letter-spacing:2px;
    }

    .hero h2{
        font-size:15px;
    }

    .profile-container{
        width:170px;
        height:170px;
    }

    .profile{
        width:155px;
        height:155px;
    }

    .about-box{
        padding:30px 20px;
    }

    .title{
        font-size:35px;
    }

}

</style>
</head>


<body>


<!-- 3D CANVAS -->

<canvas id="canvas"></canvas>


<!-- ==============================
     NAVIGATION
================================ -->

<nav>

    <div class="logo">
        HAK.
    </div>

    <ul>

        <li>
            <a href="#home">HOME</a>
        </li>

        <li>
            <a href="#about">ABOUT</a>
        </li>

        <li>
            <a href="#skills">SKILLS</a>
        </li>

        <li>
            <a href="#projects">PROJECTS</a>
        </li>

        <li>
            <a href="#education">EDUCATION</a>
        </li>

        <li>
            <a href="#contact">CONTACT</a>
        </li>

    </ul>

</nav>



<!-- ==============================
     HERO
================================ -->

<section class="hero" id="home">

    <div class="hero-content" id="heroContent">

        <div class="profile-container">

            <img
                src="IMG-20260808-WA0653.jpg"
                class="profile"
                alt="Hafees Ali K"
            >

            <div class="status"></div>

        </div>


        <h1>
            HAFEES ALI K
        </h1>


        <h2>
            BCA STUDENT • DEVELOPER • TECH ENTHUSIAST
        </h2>


        <div class="typing">

            <span id="typingText"></span>

            <span class="cursor">|</span>

        </div>


        <div class="buttons">

            <a
                href="#projects"
                class="btn"
            >
                EXPLORE PROJECTS
            </a>

            <a
                href="#contact"
                class="btn purple"
            >
                CONNECT WITH ME
            </a>

        </div>

    </div>


    <div class="scroll">
        SCROLL ↓
    </div>

</section>



<!-- ==============================
     ABOUT
================================ -->

<section id="about">

    <h2 class="title">
        ABOUT <span>ME</span>
    </h2>


    <div class="about-box">

        <p>

            I'm <strong>Hafees Ali K</strong>, currently pursuing
            my Bachelor of Computer Applications (BCA) at
            <strong>Gems Arts and Science College</strong>.

            <br><br>

            I am passionate about programming, web development,
            technology and creating futuristic digital experiences.

            <br><br>

            I enjoy learning new technologies and transforming
            ideas into creative and useful projects.

        </p>

    </div>

</section>



<!-- ==============================
     SKILLS
================================ -->

<section id="skills">

    <h2 class="title">
        MY <span>SKILLS</span>
    </h2>


    <div class="skills">


        <div class="skill-card">

            <div class="skill-icon">💻</div>

            <h3>HTML</h3>

            <p>
                Modern web structure
            </p>

        </div>


        <div class="skill-card">

            <div class="skill-icon">🎨</div>

            <h3>CSS</h3>

            <p>
                Responsive UI design
            </p>

        </div>


        <div class="skill-card">

            <div class="skill-icon">⚡</div>

            <h3>JavaScript</h3>

            <p>
                Interactive websites
            </p>

        </div>


        <div class="skill-card">

            <div class="skill-icon">🐍</div>

            <h3>Python</h3>

            <p>
                Programming & logic
            </p>

        </div>


        <div class="skill-card">

            <div class="skill-icon">🗄️</div>

            <h3>SQL</h3>

            <p>
                Database management
            </p>

        </div>


        <div class="skill-card">

            <div class="skill-icon">🚀</div>

            <h3>GitHub</h3>

            <p>
                Version control
            </p>

        </div>


    </div>

</section>



<!-- ==============================
     PROJECTS
================================ -->

<section id="projects">

    <h2 class="title">
        FEATURED <span>PROJECTS</span>
    </h2>


    <div class="projects">


        <div class="project">

            <div class="project-number">
                PROJECT 01
            </div>

            <h3>
                3D Portfolio
            </h3>

            <p>
                A futuristic personal portfolio website
                featuring animations, 3D effects and
                responsive design.
            </p>

            <a
                href="#"
                class="project-link"
            >
                VIEW PROJECT →
            </a>

        </div>


        <div class="project">

            <div class="project-number">
                PROJECT 02
            </div>

            <h3>
                Web Development
            </h3>

            <p>
                Modern responsive websites developed
                using HTML, CSS and JavaScript.
            </p>

            <a
                href="#"
                class="project-link"
            >
                VIEW PROJECT →
            </a>

        </div>


        <div class="project">

            <div class="project-number">
                PROJECT 03
            </div>

            <h3>
                Future Project
            </h3>

            <p>
                New innovative projects are currently
                being developed and will be added here.
            </p>

            <a
                href="#"
                class="project-link"
            >
                COMING SOON →
            </a>

        </div>


    </div>

</section>



<!-- ==============================
     EDUCATION
================================ -->

<section id="education">

    <h2 class="title">
        MY <span>EDUCATION</span>
    </h2>


    <div class="timeline">


        <div class="timeline-item">

            <h3>
                Bachelor of Computer Applications
            </h3>

            <p>
                Gems Arts and Science College
            </p>

            <p>
                Currently Pursuing
            </p>

        </div>


        <div class="timeline-item">

            <h3>
                Technology & Programming
            </h3>

            <p>
                Continuously learning programming,
                web development, databases and
                emerging technologies.
            </p>

        </div>


    </div>

</section>



<!-- ==============================
     CONTACT
================================ -->

<section id="contact">

    <h2 class="title">
        LET'S <span>CONNECT</span>
    </h2>


    <div class="contact">

        <p>
            Want to collaborate, discuss technology
            or check out my work? Connect with me.
        </p>


        <div class="socials">

            <!-- CHANGE THESE LINKS -->

            <a
                href="https://github.com/"
                target="_blank"
                class="social"
            >
                GitHub
            </a>


            <a
                href="https://linkedin.com/"
                target="_blank"
                class="social"
            >
                LinkedIn
            </a>


            <a
                href="mailto:yourmail@example.com"
                class="social"
            >
                Email
            </a>

        </div>

    </div>

</section>



<footer>

    © 2026
    <span>Hafees Ali K</span>
    • FUTURE IS CODE ⚡

</footer>



<script>

/* ==============================
   TYPING ANIMATION
================================ */

const texts = [

    "Building the future with code.",
    "Exploring technology and innovation.",
    "Turning ideas into digital experiences.",
    "Learning. Creating. Developing."

];

let textIndex = 0;
let charIndex = 0;

const typingElement =
    document.getElementById("typingText");

function type(){

    if(charIndex < texts[textIndex].length){

        typingElement.textContent +=
            texts[textIndex].charAt(charIndex);

        charIndex++;

        setTimeout(type,60);

    }else{

        setTimeout(erase,1800);

    }

}

function erase(){

    if(charIndex > 0){

        typingElement.textContent =
            texts[textIndex].substring(
                0,
                charIndex - 1
            );

        charIndex--;

        setTimeout(erase,30);

    }else{

        textIndex++;

        if(textIndex >= texts.length){
            textIndex = 0;
        }

        setTimeout(type,500);

    }

}

type();



/* ==============================
   3D MOUSE EFFECT
================================ */

const hero =
    document.getElementById("heroContent");

document.addEventListener("mousemove",(e)=>{

    const x =
        (window.innerWidth / 2 - e.clientX) / 40;

    const y =
        (window.innerHeight / 2 - e.clientY) / 40;

    hero.style.transform =
        `rotateY(${x}deg) rotateX(${y}deg)`;

});



/* ==============================
   3D PARTICLE SYSTEM
================================ */

const canvas =
    document.getElementById("canvas");

const ctx =
    canvas.getContext("2d");

let particles = [];

function resize(){

    canvas.width =
        window.innerWidth;

    canvas.height =
        window.innerHeight;

}

resize();

window.addEventListener(
    "resize",
    resize
);


class Particle{

    constructor(){

        this.x =
            Math.random() * canvas.width;

        this.y =
            Math.random() * canvas.height;

        this.z =
            Math.random() * 1000;

        this.size =
            Math.random() * 2 + .5;

        this.speed =
            Math.random() * 2 + .5;

    }


    update(){

        this.z -= this.speed;

        if(this.z <= 0){

            this.z = 1000;

            this.x =
                Math.random() * canvas.width;

            this.y =
                Math.random() * canvas.height;

        }

    }


    draw(){

        const scale =
            1000 / this.z;

        const x =
            (this.x - canvas.width/2)
            * scale
            + canvas.width/2;

        const y =
            (this.y - canvas.height/2)
            * scale
            + canvas.height/2;

        const size =
            this.size * scale;

        ctx.beginPath();

        ctx.arc(
            x,
            y,
            size,
            0,
            Math.PI * 2
        );

        ctx.fillStyle =
            "rgba(0,234,255,.7)";

        ctx.fill();

    }

}


for(let i=0;i<300;i++){

    particles.push(
        new Particle()
    );

}


function animate(){

    ctx.clearRect(
        0,
        0,
        canvas.width,
        canvas.height
    );

    particles.forEach(p=>{

        p.update();
        p.draw();

    });

    requestAnimationFrame(
        animate
    );

}

animate();


</script>

</body>
</html>
