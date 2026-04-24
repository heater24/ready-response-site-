# ready-response-site-
ready response training business website
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Ready Response Training</title>

  <style>
    :root{
      --green:#00cc66;
      --dark:#0a0f0a;
      --panel:#101a10;
    }

    *{box-sizing:border-box}

    body {
      margin: 0;
      font-family: Arial, sans-serif;
      color: #e6ffe6;
      background-color: var(--dark);
      background-image: url("data:image/svg+xml,%3Csvg width='400' height='400' viewBox='0 0 400 400' xmlns='http://www.w3.org/2000/svg'%3E%3Cg fill='none' stroke='%2300cc66' stroke-width='0.7' opacity='0.12'%3E%3Cpath d='M0 200 Q 100 80 200 200 T 400 200'/%3E%3Cpath d='M0 260 Q 120 140 200 260 T 400 260'/%3E%3Cpath d='M0 140 Q 120 20 200 140 T 400 140'/%3E%3Cpath d='M0 320 Q 140 200 200 320 T 400 320'/%3E%3C/g%3E%3C/svg%3E");
      background-size: 400px 400px;
    }

    header {
      background: rgba(0,0,0,0.9);
      backdrop-filter: blur(8px);
      padding: 14px 20px;
      border-bottom: 2px solid var(--green);
      position: sticky;
      top: 0;
      z-index: 10;
      display:flex;
      align-items:center;
      justify-content:space-between;
      flex-wrap:wrap;
      gap:10px;
    }

    .brand{
      display:flex;
      align-items:center;
      gap:12px;
    }

    .brand img{height:48px}

    .brand h1{
      margin:0;
      color:var(--green);
      font-size:18px;
      letter-spacing:2px;
    }

    nav {
      display:flex;
      gap:16px;
      flex-wrap:wrap;
    }

    nav a {
      color:#e6ffe6;
      text-decoration:none;
      font-weight:bold;
      font-size:14px;
    }

    nav a:hover{color:var(--green)}

    .hero {
      text-align:center;
      padding:70px 20px 50px;
    }

    .hero img.logo{
      width:200px;
      filter: drop-shadow(0 0 12px rgba(0,204,102,.35));
    }

    .hero h2 { color: var(--green); }

    .cta a {
      background: var(--green);
      color: #000;
      padding: 12px 18px;
      border-radius: 6px;
      text-decoration: none;
      font-weight: bold;
      display:inline-block;
      margin-top:10px;
    }

    .section {
      padding: 50px 20px;
      max-width: 1100px;
      margin: auto;
    }

    .section h2{color:var(--green)}

    .grid {
      display:grid;
      grid-template-columns: repeat(auto-fit, minmax(240px,1fr));
      gap:18px;
    }

    .card {
      background: rgba(16,26,16,0.95);
      padding: 18px;
      border-radius: 12px;
      border: 1px solid rgba(0,204,102,.35);
    }

    .images {
      display:grid;
      grid-template-columns: repeat(auto-fit,minmax(240px,1fr));
      gap:15px;
    }

    .images img{
      width:100%;
      height:200px;
      object-fit:cover;
      border-radius:10px;
      border:1px solid rgba(0,204,102,.25);
    }

    form {
      display:grid;
      gap:12px;
      max-width:600px;
      margin:auto;
    }

    input, select, textarea {
      padding:12px;
      border-radius:6px;
      border:none;
      background:#0f1a0f;
      color:#e6ffe6;
    }

    button {
      background:var(--green);
      color:#000;
      padding:14px;
      border:none;
      border-radius:6px;
      font-weight:bold;
      cursor:pointer;
    }

    footer {
      text-align:center;
      padding:20px;
      border-top:1px solid var(--green);
      font-size:14px;
    }
  </style>
</head>

<body>

<header>
  <div class="brand">
    <img src="logo.png" alt="Ready Response Logo" />
    <h1>READY RESPONSE</h1>
  </div>
  <nav>
    <a href="#services">Services</a>
    <a href="#industries">Industries</a>
    <a href="#booking">Book</a>
    <a href="#contact">Contact</a>
  </nav>
</header>

<section class="hero">
  <img class="logo" src="logo.png" alt="Ready Response Logo" />
  <h2>Real-World Safety Training</h2>
  <p>Oilfield • Construction • Industrial</p>
  <div class="cta">
    <a href="#booking">Schedule a Weekend Class</a>
  </div>
</section>

<section id="services" class="section">
  <h2>Training Services</h2>
  <div class="grid">
    <div class="card"><h3>CPR / AED</h3><p style="margin-top:8px; font-size:13px; color:#a8ffcc;">Max 12 students per class</p></div>
    <div class="card"><h3>First Aid</h3></div>
    <div class="card"><h3>H2S Safety</h3></div>
    <div class="card"><h3>Forklift / Scissor Lift</h3></div>
  </div>
</section>

<section id="industries" class="section">
  <h2>Industries We Serve</h2>
  <div class="images">
    <img src="https://images.unsplash.com/photo-1589792923962-537704632910?auto=format&fit=crop&w=800&q=60" alt="Pump Jack Oilfield" loading="lazy" />
    <img src="https://images.unsplash.com/photo-1590479773265-7464e5d48118?auto=format&fit=crop&w=800&q=60" alt="Construction Equipment" loading="lazy" />
    <img src="https://images.unsplash.com/photo-1581092334651-ddf26d9a09d5?auto=format&fit=crop&w=800&q=60" alt="Industrial Work" loading="lazy" />
  </div>
</section>

<section id="booking" class="section">
  <h2>Request On-Site Training (Weekends Only)</h2>
  <p>All training is conducted at your location. Weekend availability only.</p>

  <!-- NOTE: mailto is unreliable. Consider Formspree or backend email service -->
  <form action="mailto:readyresponse940@gmail.com" method="POST" enctype="text/plain">

    <input type="text" name="Name" placeholder="Full Name" required />
    <input type="text" name="Company" placeholder="Company Name" required />
    <input type="tel" name="Phone" placeholder="Phone Number" required />
    <input type="email" name="Email" placeholder="Email Address" required />
    <input type="text" name="Location" placeholder="Training Address / Job Site" required />

    <select name="Training Type" required>
      <option value="">Select Training Type</option>
      <option>CPR / AED</option>
      <option>First Aid</option>
      <option>H2S Safety</option>
      <option>Forklift / Scissor Lift</option>
          </select>

    <input type="date" name="Preferred Date" required />
    <input type="number" name="Group Size" placeholder="Number of Students" />
    <textarea name="Details" rows="4" placeholder="Additional details..."></textarea>

    <button type="submit">Submit Request</button>
  </form>

  
</section>

<section id="contact" class="section">
  <h2>Contact</h2>
  <p>(940) 841-1001</p>
  <p>readyresponse940@gmail.com</p>
</section>

<footer>
  © 2026 Ready Response | Veteran Owned Training Company
</footer>

</body>
</html>
