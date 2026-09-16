<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>CYBER ZONE | Digital Services</title>
<meta name="description" content="CYBER ZONE - Aadhaar, PAN, GST, printing, passport, railway, air ticket, AEPS and digital services.">
<style>
:root{
  --bg:#050816;--panel:rgba(10,18,38,.72);--cyan:#00eaff;--blue:#3d7cff;
  --pink:#ff27c8;--text:#eef7ff;--muted:#9fb3c8;--line:rgba(0,234,255,.22);
}
*{box-sizing:border-box;margin:0;padding:0}
html{scroll-behavior:smooth}
body{
  font-family:Arial,Helvetica,sans-serif;background:
  radial-gradient(circle at 15% 10%,rgba(0,234,255,.13),transparent 28%),
  radial-gradient(circle at 85% 25%,rgba(255,39,200,.12),transparent 25%),var(--bg);
  color:var(--text);overflow-x:hidden;
}
body:before{
 content:"";position:fixed;inset:0;pointer-events:none;opacity:.12;
 background-image:linear-gradient(rgba(0,234,255,.2) 1px,transparent 1px),linear-gradient(90deg,rgba(0,234,255,.2) 1px,transparent 1px);
 background-size:55px 55px;mask-image:linear-gradient(to bottom,black,transparent 80%);
}
a{text-decoration:none;color:inherit}
.container{width:min(1160px,92%);margin:auto}
header{
 position:sticky;top:0;z-index:20;background:rgba(3,7,20,.76);
 backdrop-filter:blur(14px);border-bottom:1px solid var(--line)
}
.nav{height:76px;display:flex;align-items:center;justify-content:space-between}
.brand{display:flex;align-items:center;gap:12px}
.logo{
 width:50px;height:50px;border:1px solid var(--cyan);border-radius:14px;
 display:grid;place-items:center;color:var(--cyan);font-weight:900;
 box-shadow:0 0 10px var(--cyan),inset 0 0 18px rgba(0,234,255,.15)
}
.brand h2{font-size:20px;letter-spacing:3px;text-shadow:0 0 12px var(--cyan)}
nav{display:flex;gap:24px;font-size:14px;color:#c7d8e8}
nav a:hover{color:var(--cyan);text-shadow:0 0 10px var(--cyan)}
.hero{min-height:680px;display:grid;place-items:center;text-align:center;padding:90px 0 70px;position:relative}
.hero .orb{position:absolute;width:360px;height:360px;border-radius:50%;border:1px solid rgba(0,234,255,.18);box-shadow:0 0 100px rgba(0,234,255,.12);animation:pulse 4s infinite}
.hero h1{font-size:clamp(45px,9vw,92px);letter-spacing:8px;line-height:1;text-shadow:0 0 12px var(--cyan),0 0 45px rgba(0,234,255,.55);animation:flicker 4s infinite}
.hero h1 span{color:var(--pink);text-shadow:0 0 12px var(--pink),0 0 35px rgba(255,39,200,.5)}
.hero p{max-width:720px;margin:24px auto;color:var(--muted);font-size:18px;line-height:1.7}
.btn{
 display:inline-block;padding:14px 24px;border:1px solid var(--cyan);border-radius:999px;
 color:#fff;background:rgba(0,234,255,.08);box-shadow:0 0 16px rgba(0,234,255,.22);
 transition:.25s;margin:7px;font-weight:700
}
.btn:hover{transform:translateY(-3px);background:var(--cyan);color:#03101a;box-shadow:0 0 30px var(--cyan)}
section{padding:85px 0}
.section-title{text-align:center;margin-bottom:42px}
.section-title h2{font-size:36px;text-shadow:0 0 14px rgba(0,234,255,.7)}
.section-title p{color:var(--muted);margin-top:10px}
.grid{display:grid;grid-template-columns:repeat(4,1fr);gap:18px}
.card{
 position:relative;padding:26px 20px;min-height:190px;border:1px solid var(--line);
 border-radius:20px;background:linear-gradient(145deg,rgba(14,27,52,.82),rgba(5,10,25,.72));
 overflow:hidden;transition:.3s
}
.card:before{content:"";position:absolute;inset:-2px;border-radius:20px;border:1px solid transparent;transition:.3s}
.card:hover{transform:translateY(-8px);border-color:var(--cyan);box-shadow:0 0 28px rgba(0,234,255,.2)}
.icon{font-size:34px;margin-bottom:15px;filter:drop-shadow(0 0 8px var(--cyan))}
.card h3{font-size:18px;margin-bottom:8px}
.card p{font-size:13px;line-height:1.55;color:var(--muted);min-height:42px}
.card .go{display:inline-block;margin-top:16px;color:var(--cyan);font-size:13px;font-weight:bold}
.notice{margin-top:30px;text-align:center;color:#a9bfd1;font-size:12px}
.contact{
 display:grid;grid-template-columns:1fr 1fr;gap:28px;align-items:stretch
}
.contact-box{padding:34px;border:1px solid var(--line);border-radius:24px;background:var(--panel);box-shadow:0 0 30px rgba(0,234,255,.08)}
.contact-box h3{font-size:25px;margin-bottom:20px}
.info{display:flex;gap:14px;padding:13px 0;border-bottom:1px solid rgba(255,255,255,.07);color:#c9d8e6}
.info b{color:var(--cyan);min-width:85px}
footer{padding:30px 0;border-top:1px solid var(--line);text-align:center;color:#8095a9;font-size:13px}
.whatsapp{
 position:fixed;right:22px;bottom:22px;z-index:30;width:58px;height:58px;border-radius:50%;
 display:grid;place-items:center;background:#13d96b;color:white;font-size:27px;
 box-shadow:0 0 25px rgba(19,217,107,.6);animation:float 2.2s infinite
}
@keyframes pulse{50%{transform:scale(1.08);opacity:.65}}
@keyframes flicker{0%,18%,22%,63%,100%{opacity:1}20%,21%,64%{opacity:.82}}
@keyframes float{50%{transform:translateY(-7px)}}
@media(max-width:900px){.grid{grid-template-columns:repeat(2,1fr)}.contact{grid-template-columns:1fr}nav{display:none}}
@media(max-width:520px){.grid{grid-template-columns:1fr}.hero{min-height:600px}.hero h1{letter-spacing:4px}.hero p{font-size:15px}}
</style>
</head>
<body>

<header>
 <div class="container nav">
  <a class="brand" href="#home">
   <!-- REPLACE THIS BOX WITH YOUR CYBER ZONE LOGO IMAGE LATER -->
   <div class="logo">CZ</div>
   <h2>CYBER ZONE</h2>
  </a>
  <nav>
   <a href="#home">Home</a><a href="#services">Services</a><a href="#contact">Contact</a>
  </nav>
 </div>
</header>

<main id="home">
<section class="hero">
 <div class="orb"></div>
 <div class="container" style="position:relative;z-index:2">
  <div style="color:var(--cyan);letter-spacing:4px;font-size:12px;margin-bottom:18px">DIGITAL SERVICE • PRINT • TRAVEL</div>
  <h1>CYBER <span>ZONE</span></h1>
  <p>One-stop digital service centre for government services, documentation, printing, travel booking and everyday online work.</p>
  <a class="btn" href="#services">EXPLORE SERVICES</a>
  <a class="btn" href="#contact">CONTACT US</a>
 </div>
</section>

<section id="services">
 <div class="container">
  <div class="section-title">
   <h2>OUR SERVICES</h2>
   <p>Click any service to open its official portal.</p>
  </div>
  <div class="grid">

   <a class="card" href="https://www.uidai.gov.in/" target="_blank" rel="noopener">
    <div class="icon">🪪</div><h3>Aadhaar</h3><p>Download, update and access Aadhaar services.</p><span class="go">OFFICIAL PORTAL →</span>
   </a>

   <a class="card" href="https://www.incometax.gov.in/" target="_blank" rel="noopener">
    <div class="icon">💳</div><h3>PAN Card</h3><p>PAN-related information and Income Tax services.</p><span class="go">OFFICIAL PORTAL →</span>
   </a>

   <a class="card" href="https://www.gst.gov.in/" target="_blank" rel="noopener">
    <div class="icon">🧾</div><h3>GST</h3><p>GST registration, returns and taxpayer services.</p><span class="go">OFFICIAL PORTAL →</span>
   </a>

   <a class="card" href="#contact">
    <div class="icon">🖨️</div><h3>Printing & Scanning</h3><p>Colour/B&W printing, scanning, photocopy and document work.</p><span class="go">ENQUIRE NOW →</span>
   </a>

   <a class="card" href="#contact">
    <div class="icon">📸</div><h3>Photo & Passport Photo</h3><p>Digital photo, passport-size photo and document photo services.</p><span class="go">ENQUIRE NOW →</span>
   </a>

   <a class="card" href="https://www.passportindia.gov.in/" target="_blank" rel="noopener">
    <div class="icon">🛂</div><h3>Passport</h3><p>Passport application information and official services.</p><span class="go">OFFICIAL PORTAL →</span>
   </a>

   <a class="card" href="https://www.irctc.co.in/" target="_blank" rel="noopener">
    <div class="icon">🚆</div><h3>Railway Ticket</h3><p>Indian Railway ticket booking through IRCTC.</p><span class="go">IRCTC →</span>
   </a>

   <a class="card" href="#contact">
    <div class="icon">✈️</div><h3>Air Ticket</h3><p>Domestic and international air-ticket booking assistance.</p><span class="go">BOOKING ENQUIRY →</span>
   </a>

   <a class="card" href="#contact">
    <div class="icon">💰</div><h3>AEPS</h3><p>Aadhaar Enabled Payment System and assisted banking services.</p><span class="go">CONTACT US →</span>
   </a>

   <a class="card" href="https://beneficiary.nha.gov.in/" target="_blank" rel="noopener">
    <div class="icon">🏥</div><h3>Ayushman Card</h3><p>Access the official Ayushman beneficiary portal.</p><span class="go">OFFICIAL PORTAL →</span>
   </a>

   <a class="card" href="#contact">
    <div class="icon">🏠</div><h3>Jamin Ka Lagan</h3><p>Land-revenue related online assistance and documentation.</p><span class="go">ENQUIRE NOW →</span>
   </a>

   <a class="card" href="#contact">
    <div class="icon">👷</div><h3>PF / EPFO</h3><p>PF-related online assistance and documentation support.</p><span class="go">ENQUIRE NOW →</span>
   </a>

   <a class="card" href="https://parivahan.gov.in/" target="_blank" rel="noopener">
    <div class="icon">🚘</div><h3>Driving Licence</h3><p>Parivahan services and driving-licence assistance.</p><span class="go">OFFICIAL PORTAL →</span>
   </a>

   <a class="card" href="#contact">
    <div class="icon">🛡️</div><h3>Vehicle Insurance</h3><p>Vehicle insurance assistance and document services.</p><span class="go">ENQUIRE NOW →</span>
   </a>

   <a class="card" href="#contact">
    <div class="icon">📄</div><h3>Online Forms</h3><p>Online applications, form filling and document uploading.</p><span class="go">ENQUIRE NOW →</span>
   </a>

   <a class="card" href="#contact">
    <div class="icon">💻</div><h3>Other Digital Services</h3><p>Ask us about additional online and documentation services.</p><span class="go">CONTACT US →</span>
   </a>
  </div>
  <div class="notice">Official portals open in a new tab. CYBER ZONE provides assisted digital-service support and is not a government department.</div>
 </div>
</section>

<section id="contact">
 <div class="container">
  <div class="section-title"><h2>CONTACT CYBER ZONE</h2><p>Visit us or contact us for assistance.</p></div>
  <div class="contact">
   <div class="contact-box">
    <h3>📍 Visit Our Centre</h3>
    <div class="info"><b>Address</b><span>Main Road, Goush Nagar, Makhdumpur, Bokaro</span></div>
    <div class="info"><b>Phone</b><span>YOUR PHONE NUMBER</span></div>
    <div class="info"><b>WhatsApp</b><span>YOUR WHATSAPP NUMBER</span></div>
    <div class="info"><b>Hours</b><span>YOUR OPENING HOURS</span></div>
   </div>
   <div class="contact-box">
    <h3>💬 Need a Service?</h3>
    <p style="color:var(--muted);line-height:1.8">Send your query or document requirements to CYBER ZONE. We will assist you with the available service.</p>
    <a class="btn" href="https://wa.me/YOURNUMBER" target="_blank" rel="noopener">WHATSAPP US</a>
    <a class="btn" href="tel:YOURNUMBER">CALL NOW</a>
   </div>
  </div>
 </div>
</section>
</main>

<a class="whatsapp" href="https://wa.me/YOURNUMBER" target="_blank" rel="noopener" aria-label="WhatsApp">☏</a>

<footer>© 2026 CYBER ZONE • Digital Services • All Rights Reserved</footer>
</body>
</html>
