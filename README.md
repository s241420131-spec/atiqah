
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Kg Wai Adventure</title>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@300;400;500;600;700&display=swap" rel="stylesheet">

<style>

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:'Montserrat',sans-serif;
    scroll-behavior:smooth;
}

body{
    background-image:url('https://images.unsplash.com/photo-1506744038136-46273834b3fb?q=80&w=2000&auto=format&fit=crop');
    background-size:cover;
    background-position:center;
    background-repeat:no-repeat;
    background-attachment:fixed;
    color:#222;
    overflow-x:hidden;
}

header{
    position:fixed;
    top:0;
    width:100%;
    z-index:999;
    background:rgba(20,20,20,0.45);
    backdrop-filter:blur(12px);
    padding:18px 70px;
}

nav{
    display:flex;
    justify-content:space-between;
    align-items:center;
}

.logo{
    color:white;
    font-size:30px;
    font-weight:700;
    letter-spacing:2px;
}

nav ul{
    display:flex;
    gap:35px;
    list-style:none;
}

nav ul li a{
    color:white;
    text-decoration:none;
    font-size:15px;
    transition:0.3s;
}

nav ul li a:hover{
    color:#d6ad60;
}

.hero{
    height:100vh;
    background:linear-gradient(135deg,#1f1f1f,#5c4432,#d6ad60);
    background-size:cover;
    background-position:center;
    display:flex;
    justify-content:center;
    align-items:center;
    text-align:center;
    color:white;
    padding:20px;
}

.hero-content h1{
    font-size:85px;
    font-weight:700;
    margin-bottom:20px;
    letter-spacing:2px;
}

.hero-content p{
    font-size:22px;
    max-width:750px;
    margin:auto;
    margin-bottom:35px;
    line-height:1.8;
}

.btn{
    display:inline-block;
    padding:15px 40px;
    border-radius:50px;
    background:#d6ad60;
    color:white;
    text-decoration:none;
    font-weight:600;
    transition:0.4s;
}

.btn:hover{
    transform:translateY(-5px);
    background:#b58a3f;
}

section{
    padding:120px 90px;
}

.container{
    max-width:1200px;
    margin:auto;
}

.title{
    text-align:center;
    font-size:48px;
    margin-bottom:70px;
    color:#2d2016;
    position:relative;
}

.title::after{
    content:'';
    width:100px;
    height:4px;
    background:#d6ad60;
    position:absolute;
    left:50%;
    transform:translateX(-50%);
    bottom:-18px;
    border-radius:10px;
}

.about{
    margin-top:20px;
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:60px;
    align-items:center;
}



.about-text{
    backdrop-filter:blur(10px);
    background:rgba(255,255,255,0.78);
    padding:60px;
    border-radius:30px;
    width:100%;
    min-height:550px;
    display:flex;
    flex-direction:column;
    justify-content:center;
    box-shadow:0 10px 30px rgba(0,0,0,0.08);
}

.about-text h3{
    font-size:40px;
    margin-bottom:25px;
    color:#2d2016;
}

.about-text p{
    margin-bottom:15px;
    font-size:17px;
    line-height:1.9;
}

.services{
    background:rgba(239,229,216,0.75);
    backdrop-filter:blur(6px);
}

.cards{
    margin-top:20px;
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(320px,1fr));
    gap:35px;
}

.card{
    background:rgba(255,255,255,0.78);
    border-radius:30px;
    overflow:hidden;
    transition:0.4s;
    box-shadow:0 15px 30px rgba(0,0,0,0.08);
}

.card:hover{
    transform:translateY(-12px);
}



.card-content{
    padding:35px;
}

.card-content h3{
    font-size:28px;
    margin-bottom:18px;
    color:#2d2016;
}

.card-content p{
    line-height:1.8;
}

.gallery-grid{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
    gap:25px;
}





.video{
    background:#1f1f1f;
    text-align:center;
}

.video .title{
    color:white;
}

iframe{
    width:85%;
    height:550px;
    border:none;
    border-radius:30px;
    box-shadow:0 15px 40px rgba(0,0,0,0.35);
}

.contact-box{
    backdrop-filter:blur(10px);
    margin-top:20px;
    max-width:800px;
    margin:auto;
    background:rgba(255,255,255,0.78);
    padding:60px;
    border-radius:35px;
    text-align:center;
    box-shadow:0 10px 30px rgba(0,0,0,0.08);
}

.contact-box p{
    margin:18px 0;
    font-size:20px;
}

footer{
    background:#1f1f1f;
    color:white;
    text-align:center;
    padding:30px;
    letter-spacing:1px;
}

@media(max-width:900px){

    header{
        padding:18px 30px;
    }

    nav{
        flex-direction:column;
        gap:15px;
    }

    nav ul{
        gap:18px;
        flex-wrap:wrap;
        justify-content:center;
    }

    .hero-content h1{
        font-size:50px;
    }

    .hero-content p{
        font-size:18px;
    }

    section{
        padding:90px 25px;
    }

    .about{
        grid-template-columns:1fr;
    }

    .about img{
        height:420px;
    }

    iframe{
        width:100%;
        height:320px;
    }

}

</style>
</head>
<body>

<header>
<nav>
<div class="logo">KG WAI</div>

<ul>
<li><a href="#home">HOME</a></li>
<li><a href="#about">ABOUT</a></li>
<li><a href="#services">SERVICES</a></li>

<li><a href="#contact">CONTACT</a></li>
</ul>

</nav>
</header>

<section class="hero" id="home">

<div class="hero-content">
<h1>KG WAI ADVENTURE</h1>

<p>
Experience the calm beauty of nature with boat rides,
kayak adventures and relaxing village tourism in Perlis.
</p>

<a href="#gallery" class="btn">DISCOVER NOW</a>
</div>

</section>

<section id="about">
<div class="container">

<h2 class="title">About The Operator</h2>

<div class="about">



<div class="about-text">

<h3>Kamarulzaman bin Ahmad</h3>

<p><strong>Age:</strong> 36 Years Old</p>
<p><strong>Origin:</strong> Perlis</p>
<p><strong>Position:</strong> PIC (Person In Charge)</p>
<p><strong>Experience:</strong> 1 Year</p>

<br>

<p>
Managing tourism activities around Kg Wai including
boat rides, kayak adventures and visitor experiences.
Activities are available during weekdays, weekends and school holidays.
</p>

</div>

</div>

</div>
</section>

<section class="services" id="services">
<div class="container">

<h2 class="title">Our Services</h2>

<div class="cards">

<div class="card">


<div class="card-content">
<h3>Boat Trip</h3>
<p>
Relaxing river journey from Kg Wai to Tebing Tinggi.
Perfect for nature lovers and family activities.
</p>
</div>
</div>

<div class="card">


<div class="card-content">
<h3>Kayak Adventure</h3>
<p>
Fun kayak experience surrounded by peaceful scenery
and beautiful village landscapes.
</p>
</div>
</div>

<div class="card">


<div class="card-content">
<h3>Village Tourism</h3>
<p>
Discover the authentic lifestyle and tourism attractions
available around Kg Wai, Perlis.
</p>
</div>
</div>

</div>

</div>
</section>

<section id="contact">
<div class="container">

<h2 class="title">Contact</h2>

<div class="contact-box">

<p><strong>Location:</strong> Kg Wai, Perlis</p>
<p><strong>Activities:</strong> Boat Ride & Kayak Tourism</p>
<p><strong>Available:</strong> Weekdays & Weekends</p>
<p><strong>Email:</strong> kgwaiadventure@gmail.com</p>

</div>

</div>
</section>

<footer>

<p>© 2026 KG WAI ADVENTURE | PERSONAL WEBSITE</p>

</footer>

</body>
</html>
