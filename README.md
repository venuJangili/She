<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />

    <title>She Can Foundation</title>

    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">

    <style>

        *{
            margin:0;
            padding:0;
            box-sizing:border-box;
            scroll-behavior:smooth;
        }

        body{
            font-family:'Poppins',sans-serif;
            background:#f5f7fb;
            color:#222;
        }

        /* NAVBAR */

        header{
            width:100%;
            position:fixed;
            top:0;
            left:0;
            z-index:1000;
            background:rgba(255,255,255,0.95);
            backdrop-filter:blur(10px);
            box-shadow:0 2px 10px rgba(0,0,0,0.08);
        }

        .navbar{
            width:90%;
            margin:auto;
            display:flex;
            justify-content:space-between;
            align-items:center;
            padding:18px 0;
        }

        .logo{
            font-size:28px;
            font-weight:700;
            color:#6c63ff;
        }

        .nav-links{
            display:flex;
            gap:30px;
        }

        .nav-links a{
            text-decoration:none;
            color:#333;
            font-weight:500;
            transition:0.3s;
        }

        .nav-links a:hover{
            color:#6c63ff;
        }

        /* HERO SECTION */

        .hero{
            min-height:100vh;
            display:flex;
            justify-content:center;
            align-items:center;
            padding:120px 10%;
            gap:60px;
            background:linear-gradient(to right,#eef2ff,#ffffff);
            flex-wrap:wrap;
        }

        .hero-text{
            flex:1;
            min-width:300px;
            animation:fadeInLeft 1s ease;
        }

        .hero-text h1{
            font-size:55px;
            line-height:1.2;
            margin-bottom:20px;
            color:#222;
        }

        .hero-text span{
            color:#6c63ff;
        }

        .hero-text p{
            font-size:18px;
            line-height:1.8;
            margin-bottom:30px;
            color:#555;
        }

        .buttons{
            display:flex;
            gap:20px;
            flex-wrap:wrap;
        }

        .btn{
            padding:14px 30px;
            border:none;
            border-radius:50px;
            cursor:pointer;
            font-size:16px;
            font-weight:600;
            transition:0.3s;
        }

        .primary-btn{
            background:#6c63ff;
            color:white;
        }

        .primary-btn:hover{
            background:#5548f5;
            transform:translateY(-3px);
        }

        .secondary-btn{
            background:white;
            border:2px solid #6c63ff;
            color:#6c63ff;
        }

        .secondary-btn:hover{
            background:#6c63ff;
            color:white;
        }

        .hero-image{
            flex:1;
            min-width:300px;
            text-align:center;
            animation:fadeInRight 1s ease;
        }

        .hero-image img{
            width:100%;
            max-width:500px;
            border-radius:20px;
            box-shadow:0 10px 30px rgba(0,0,0,0.15);
        }

        /* ABOUT SECTION */

        .about{
            padding:100px 10%;
            background:white;
        }

        .section-title{
            text-align:center;
            margin-bottom:60px;
        }

        .section-title h2{
            font-size:40px;
            color:#6c63ff;
            margin-bottom:10px;
        }

        .section-title p{
            color:#666;
        }

        .about-container{
            display:grid;
            grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
            gap:30px;
        }

        .card{
            background:#f8f9ff;
            padding:30px;
            border-radius:18px;
            transition:0.3s;
            box-shadow:0 5px 15px rgba(0,0,0,0.05);
        }

        .card:hover{
            transform:translateY(-10px);
        }

        .card h3{
            margin-bottom:15px;
            color:#6c63ff;
        }

        .card p{
            line-height:1.7;
            color:#555;
        }

        /* JOIN SECTION */

        .join{
            padding:100px 10%;
            text-align:center;
            background:linear-gradient(to right,#6c63ff,#8b85ff);
            color:white;
        }

        .join h2{
            font-size:42px;
            margin-bottom:20px;
        }

        .join p{
            max-width:700px;
            margin:auto;
            line-height:1.8;
            margin-bottom:30px;
        }

        /* FOOTER */

        footer{
            background:#111827;
            color:white;
            padding:30px 10%;
            text-align:center;
        }

        footer p{
            margin:8px 0;
            color:#d1d5db;
        }

        /* SCROLL BUTTON */

        .scroll-top{
            position:fixed;
            right:20px;
            bottom:20px;
            background:#6c63ff;
            color:white;
            border:none;
            width:45px;
            height:45px;
            border-radius:50%;
            cursor:pointer;
            display:none;
            font-size:20px;
        }

        /* ANIMATIONS */

        @keyframes fadeInLeft{
            from{
                opacity:0;
                transform:translateX(-50px);
            }
            to{
                opacity:1;
                transform:translateX(0);
            }
        }

        @keyframes fadeInRight{
            from{
                opacity:0;
                transform:translateX(50px);
            }
            to{
                opacity:1;
                transform:translateX(0);
            }
        }

        /* RESPONSIVE */

        @media(max-width:768px){

            .hero{
                text-align:center;
            }

            .hero-text h1{
                font-size:38px;
            }

            .buttons{
                justify-content:center;
            }

            .nav-links{
                gap:15px;
            }

        }

    </style>
</head>

<body>

    <!-- HEADER -->

    <header>

        <div class="navbar">

            <div class="logo">
                She Can Foundation
            </div>

            <div class="nav-links">
                <a href="#home">Home</a>
                <a href="#about">About</a>
                <a href="#join">Join Us</a>
            </div>

        </div>

    </header>

    <!-- HERO SECTION -->

    <section class="hero" id="home">

        <div class="hero-text">

            <h1>
                Empowering <span>Students</span> Through Learning & Opportunities
            </h1>

            <p>
                She Can Foundation is a youth-driven NGO creating positive social impact
                through education, digital initiatives, and community programs.
                We believe every student deserves opportunities to learn, grow,
                and showcase their talent confidently.
            </p>

            <div class="buttons">

                <button class="btn primary-btn" onclick="joinMessage()">
                    Volunteer Now
                </button>

                <button class="btn secondary-btn">
                    Learn More
                </button>

            </div>

        </div>

        <div class="hero-image">

            <img src="https://images.unsplash.com/photo-1522202176988-66273c2fd55f?w=1000"
                 alt="Students">

        </div>

    </section>

    <!-- ABOUT SECTION -->

    <section class="about" id="about">

        <div class="section-title">

            <h2>About Us</h2>

            <p>
                Building opportunities for students through technology, education, and community support.
            </p>

        </div>

        <div class="about-container">

            <div class="card">

                <h3>Education</h3>

                <p>
                    We provide practical learning opportunities and internships
                    to help students improve their real-world skills.
                </p>

            </div>

            <div class="card">

                <h3>Digital Initiatives</h3>

                <p>
                    Our programs encourage creativity, innovation,
                    and technology-driven solutions for social impact.
                </p>

            </div>

            <div class="card">

                <h3>Community Support</h3>

                <p>
                    We believe in teamwork, leadership, and empowering youth
                    to contribute positively to society.
                </p>

            </div>

        </div>

    </section>

    <!-- JOIN SECTION -->

    <section class="join" id="join">

        <h2>Become A Volunteer</h2>

        <p>
            Join our mission to inspire students, create awareness,
            and make a difference through impactful community initiatives.
        </p>

        <button class="btn primary-btn" onclick="joinMessage()">
            Join Our Community
        </button>

    </section>

    <!-- FOOTER -->

    <footer>

        <p>
            © 2026 She Can Foundation. All Rights Reserved.
        </p>

        <p>
            Designed By Venu
        </p>

    </footer>

    <!-- SCROLL TOP BUTTON -->

    <button class="scroll-top" id="scrollBtn">
        ↑
    </button>

    <!-- JAVASCRIPT -->

    <script>

        function joinMessage(){
            alert("Thank You For Your Interest In She Can Foundation!");
        }

        const scrollBtn = document.getElementById("scrollBtn");

        window.onscroll = function(){

            if(document.body.scrollTop > 300 || document.documentElement.scrollTop > 300){
                scrollBtn.style.display = "block";
            }
            else{
                scrollBtn.style.display = "none";
            }

        };

        scrollBtn.addEventListener("click", function(){

            window.scrollTo({
                top:0,
                behavior:"smooth"
            });

        });

    </script>

</body>
</html>
