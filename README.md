# Diptarafder_Official.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dip Tarafder | Official Portfolio</title>
    
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;700;900&family=Playfair+Display:ital,wght@1,700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.2/css/all.min.css">
    
    <style>
        :root {
            --tiger-orange: #ff8c00;
            --deep-purple: #6d28d9;
            --glass-white: rgba(255, 255, 255, 0.9);
            --dark-text: #1a1a1a;
        }

        body { font-family: 'Inter', sans-serif; margin: 0; color: var(--dark-text); background: #ffffff; }

        /* Navigation */
        nav { 
            padding: 1.2rem 8%; 
            display: flex; 
            justify-content: space-between; 
            align-items: center; 
            background: #fff;
            box-shadow: 0 2px 10px rgba(0,0,0,0.05);
        }
        .logo { font-weight: 900; font-size: 1.3rem; text-transform: uppercase; }

        /* High-Contrast Hero Section */
        .hero {
            background: linear-gradient(rgba(45, 10, 80, 0.5), rgba(0, 0, 0, 0.7)), 
                        url('https://images.unsplash.com/photo-1550684848-fac1c5b4e853?q=80&w=1920'); 
            background-size: cover;
            background-attachment: fixed;
            padding: 100px 10%;
            display: flex;
            align-items: center;
            justify-content: center;
            flex-wrap: wrap;
            color: white;
            text-shadow: 2px 2px 10px rgba(0,0,0,0.5);
        }
        .hero-profile {
            width: 300px;
            height: 300px;
            border-radius: 50%;
            border: 12px solid rgba(255,255,255,0.15);
            overflow: hidden;
            margin-right: 50px;
            box-shadow: 0 20px 40px rgba(0,0,0,0.4);
        }
        .hero-profile img { width: 100%; height: 100%; object-fit: cover; }
        
        .hero-text .sub { font-family: 'Playfair Display', serif; font-size: 2.8rem; color: var(--tiger-orange); font-style: italic; margin: 0; }
        .hero-text .label { color: #ffd700; font-size: 0.8rem; letter-spacing: 4px; font-weight: 900; margin: 10px 0; display: block; }
        .hero-text h1 { font-size: 4rem; font-weight: 900; margin: 0; line-height: 1; text-transform: uppercase; }

        /* Saturated Need Me Section */
        .need-me { 
            background: #e0e0e0; 
            padding: 100px 0; 
            text-align: center; 
            background-image: url('https://www.transparenttextures.com/patterns/cubes.png');
        }
        .need-me h2 { font-size: 4rem; font-weight: 900; margin: 0; color: #000; }
        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 25px;
            padding: 50px 10% 0;
        }
        .card { 
            background: var(--glass-white); 
            padding: 50px 40px; 
            text-align: left; 
            border-radius: 4px;
            box-shadow: 0 15px 35px rgba(0,0,0,0.1);
            transition: transform 0.3s;
        }
        .card:hover { transform: translateY(-10px); }
        .card i { color: var(--deep-purple); font-size: 2rem; margin-bottom: 25px; display: block; }
        .card h3 { font-size: 0.9rem; color: #666; border-bottom: 2px solid #eee; padding-bottom: 15px; margin-bottom: 20px; text-transform: uppercase; font-weight: 900; }
        .card p strong { font-size: 1.5rem; display: block; color: #000; margin-bottom: 8px; }

        /* Hobby Saturated */
        .hobby { padding: 100px 10%; text-align: center; background: #fff; }
        .hobby h2 { font-size: 4.5rem; font-weight: 900; margin-bottom: 40px; color: #111; }
        .hobby-box { 
            width: 100%; max-width: 900px; height: 500px; 
            background: linear-gradient(45deg, #111, #333);
            margin: 0 auto; border-radius: 15px; box-shadow: 0 30px 60px rgba(0,0,0,0.3);
            display: flex; align-items: center; justify-content: center; overflow: hidden;
        }

        /* About Me Vivid Purple */
        .about { 
            background: linear-gradient(135deg, #7c3aed, #4c1d95); 
            color: white; padding: 120px 10%; text-align: center; 
        }
        .about img { 
            width: 280px; height: 280px; border-radius: 50%; 
            border: 8px solid rgba(255,255,255,0.3); 
            margin-bottom: 40px; box-shadow: 0 20px 40px rgba(0,0,0,0.3);
        }
        .about h2 { font-family: 'Playfair Display', serif; font-size: 3.5rem; font-style: italic; margin: 0; }
        .about .title { font-weight: 900; letter-spacing: 2px; display: block; margin: 20px 0; color: #ffd700; }
        .about p { max-width: 800px; margin: 0 auto; font-size: 1.1rem; line-height: 1.8; opacity: 0.95; }

        /* Contact Section */
        .contact { padding: 100px 10%; text-align: center; }
        .contact h2 { font-family: 'Playfair Display', serif; font-size: 4rem; font-style: italic; }
        .map { width: 100%; height: 400px; background: #f0f0f0; margin: 50px 0; border: 1px solid #ddd; }
        
        .input-group { max-width: 700px; margin: 0 auto; }
        input, textarea { 
            width: 100%; padding: 20px; margin-bottom: 20px; border: 2px solid #eee; 
            border-radius: 8px; font-size: 1rem; transition: border-color 0.3s;
        }
        input:focus { border-color: var(--deep-purple); outline: none; }
        .btn { 
            background: var(--deep-purple); color: white; border: none; 
            padding: 18px 60px; font-weight: 900; font-size: 1.1rem; 
            text-transform: uppercase; cursor: pointer; border-radius: 50px;
            box-shadow: 0 10px 20px rgba(109, 40, 217, 0.3);
        }

        footer { padding: 50px; text-align: center; background: #111; color: #555; font-weight: 700; }

        @media (max-width: 768px) {
            .hero-text h1 { font-size: 2.8rem; }
            .hero-profile { width: 220px; height: 220px; margin: 0 0 30px 0; }
            .about h2, .contact h2 { font-size: 2.8rem; }
        }
    </style>
</head>
<body>

    <nav>
        <div class="logo">DIP TARAFDER.</div>
        <i class="fa fa-bars" style="font-size: 1.5rem;"></i>
    </nav>

    <header class="hero">
        <div class="hero-profile">
            <img src="IMG_20260211_182145.jpg" alt="Dip Tarafder">
        </div>
        <div class="hero-text">
            <p class="sub">Dips Officials</p>
            <span class="label">A PAGE FOR OWN-PUBLICATIONS</span>
            <h1>A SELF MADE <br> PROGRAMMER</h1>
        </div>
    </header>

    <section class="need-me">
        <h2>NEED ME</h2>
        <p style="font-weight: 900; color: #444;">THEN JUST CONNECT</p>
        <div class="grid">
            <div class="card">
                <i class="fa-solid fa-clock-rotate-left"></i>
                <h3>AGE</h3>
                <p><strong>19+</strong></p>
                <p>Experience tells stories Not the Age Of number.</p>
            </div>
            <div class="card">
                <i class="fa-solid fa-calendar-check"></i>
                <h3>DATE-OF-BIRTH</h3>
                <p><strong>18/10/2005</strong></p>
                <p>The Day was Tuesday.</p>
            </div>
            <div class="card">
                <i class="fa-solid fa-bolt"></i>
                <h3>RELATIONSHIPS INFO.</h3>
                <p><strong>SINGLE+</strong></p>
                <p>not interested.</p>
            </div>
            <div class="card">
                <i class="fa-solid fa-handshake-angle"></i>
                <h3>HELP.IN</h3>
                <p><strong>Tap to Get In</strong></p>
                <p>For Any projects or Anything about Programme</p>
            </div>
        </div>
    </section>

    <section class="hobby">
        <h2>Hobby</h2>
        <div class="hobby-box">
            <i class="fa-solid fa-guitar" style="font-size: 8rem; color: #fff; opacity: 0.1;"></i>
        </div>
    </section>

    <section class="about">
        <img src="Dip.jpg" alt="Dip Profile">
        <h2>About me</h2>
        <span class="title">UI / UX DESIGNER & WEB DEVELOPER</span>
        <p>
            Mike Adamson is a freelance designer & developer from California. Now I'm living in Los Angeles. 
            I like the ways people communicate, such as text, media content, pictures, sites, and so on. 
            My inspiration is music, old films, and my friends.
        </p>
        <button style="margin-top:40px; background:none; border:2px solid #fff; color:#fff; padding:15px 40px; font-weight:900; cursor:pointer; border-radius:5px;">CONTACT ME</button>
    </section>

    <section class="contact">
        <h2>Contacts</h2>
        <p style="font-weight: 700; color: #888;">As path you want</p>
        
        <div style="margin: 50px 0; font-size: 1.2rem;">
            <p><strong>Address:</strong> NAGARPUR, TANGAIL, BANGLADESH</p>
            <p><strong>Phone:</strong> +8801704235825</p>
            <p><strong>E-mail:</strong> diptarafd3t@gmail.com</p>
        </div>

        <div class="map"></div>

        <div class="input-group">
            <input type="text" placeholder="Name">
            <input type="email" placeholder="E-mail Address">
            <input type="text" placeholder="Your Phone">
            <textarea rows="6" placeholder="Message Dip.me"></textarea>
            <button class="btn">Send Now</button>
        </div>
    </section>

    <footer>
        <p>&copy; 2026 Dip Tarafder | All Rights Reserved</p>
    </footer>
