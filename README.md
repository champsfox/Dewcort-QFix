<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Dewcort-QFix | Verified MEPF Technicians Across Nigeria</title>
  <meta name="description" content="Book professional MEPF services anywhere in Nigeria with Dewcort Engineering Ltd." />

  <style>
    :root {
      --orange: #f58220;
      --orange-dark: #d9680d;
      --black: #151515;
      --charcoal: #242424;
      --gray: #666;
      --light: #f6f6f6;
      --white: #ffffff;
      --border: #e8e8e8;
      --success: #16834b;
      --shadow: 0 15px 45px rgba(0,0,0,.08);
      --radius: 18px;
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      font-family: Inter, Arial, sans-serif;
      color: var(--black);
      background: var(--white);
      line-height: 1.6;
    }

    a {
      color: inherit;
      text-decoration: none;
    }

    button,
    input,
    select,
    textarea {
      font: inherit;
    }

    .container {
      width: min(1180px, 92%);
      margin: auto;
    }

    /* NAVBAR */
    header {
      position: sticky;
      top: 0;
      z-index: 1000;
      background: rgba(255,255,255,.96);
      backdrop-filter: blur(12px);
      border-bottom: 1px solid var(--border);
    }

    .nav {
      min-height: 76px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 25px;
    }

    .logo {
      display: flex;
      align-items: center;
      gap: 12px;
      font-weight: 900;
      font-size: 20px;
    }

    .logo img {
      width: 145px;
      max-height: 55px;
      object-fit: contain;
    }

    .nav-links {
      display: flex;
      align-items: center;
      gap: 25px;
      font-weight: 600;
      font-size: 14px;
    }

    .nav-links a:hover {
      color: var(--orange);
    }

    .btn {
      border: none;
      border-radius: 10px;
      padding: 13px 20px;
      cursor: pointer;
      font-weight: 800;
      transition: .2s ease;
      display: inline-block;
    }

    .btn-primary {
      color: white;
      background: var(--orange);
    }

    .btn-primary:hover {
      background: var(--orange-dark);
      transform: translateY(-2px);
    }

    .btn-dark {
      background: var(--black);
      color: white;
    }

    .btn-outline {
      background: white;
      color: var(--black);
      border: 1px solid var(--border);
    }

    /* HERO */
    .hero {
      background:
        radial-gradient(circle at 90% 20%, rgba(245,130,32,.20), transparent 30%),
        linear-gradient(135deg, #fff 0%, #f8f8f8 100%);
      padding: 90px 0 75px;
    }

    .hero-grid {
      display: grid;
      grid-template-columns: 1.15fr .85fr;
      gap: 60px;
      align-items: center;
    }

    .eyebrow {
      display: inline-block;
      background: #fff2e7;
      color: var(--orange-dark);
      border: 1px solid #ffd6b5;
      padding: 7px 13px;
      border-radius: 50px;
      font-size: 12px;
      font-weight: 900;
      text-transform: uppercase;
      letter-spacing: .7px;
      margin-bottom: 20px;
    }

    h1 {
      font-size: clamp(42px, 6vw, 72px);
      line-height: 1.02;
      letter-spacing: -3px;
      margin-bottom: 24px;
    }

    h1 span {
      color: var(--orange);
    }

    .hero p {
      font-size: 19px;
      color: var(--gray);
      max-width: 680px;
      margin-bottom: 30px;
    }

    .hero-buttons {
      display: flex;
      gap: 12px;
      flex-wrap: wrap;
    }

    .hero-card {
      background: var(--black);
      color: white;
      border-radius: 28px;
      padding: 32px;
      box-shadow: var(--shadow);
      position: relative;
      overflow: hidden;
    }

    .hero-card::after {
      content: "";
      position: absolute;
      width: 220px;
      height: 220px;
      border-radius: 50%;
      background: var(--orange);
      opacity: .15;
      right: -80px;
      top: -80px;
    }

    .hero-card h3 {
      font-size: 26px;
      margin-bottom: 10px;
    }

    .hero-card p {
      color: #ccc;
      font-size: 15px;
    }

    .coverage {
      display: grid;
      grid-template-columns: repeat(3,1fr);
      gap: 10px;
      margin-top: 28px;
    }

    .coverage div {
      padding: 15px;
      background: rgba(255,255,255,.08);
      border-radius: 12px;
    }

    .coverage strong {
      display: block;
      color: var(--orange);
      font-size: 25px;
    }

    .coverage small {
      color: #bbb;
    }

    /* SECTIONS */
    section {
      padding: 80px 0;
    }

    .section-head {
      text-align: center;
      max-width: 750px;
      margin: 0 auto 45px;
    }

    .section-head h2 {
      font-size: clamp(30px, 4vw, 45px);
      line-height: 1.1;
      margin-bottom: 12px;
    }

    .section-head p {
      color: var(--gray);
    }

    /* FILTER */
    .filters {
      display: flex;
      gap: 8px;
      overflow-x: auto;
      padding-bottom: 10px;
      margin-bottom: 30px;
    }

    .filter {
      white-space: nowrap;
      border: 1px solid var(--border);
      background: white;
      padding: 10px 15px;
      border-radius: 50px;
      cursor: pointer;
      font-weight: 700;
      color: #444;
    }

    .filter.active,
    .filter:hover {
      background: var(--orange);
      border-color: var(--orange);
      color: white;
    }

    /* SERVICES */
    .service-grid {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 20px;
    }

    .service-card {
      border: 1px solid var(--border);
      border-radius: var(--radius);
      padding: 25px;
      background: white;
      transition: .25s;
    }

    .service-card:hover {
      transform: translateY(-5px);
      box-shadow: var(--shadow);
      border-color: #ffd4b2;
    }

    .service-icon {
      width: 50px;
      height: 50px;
      border-radius: 14px;
      display: grid;
      place-items: center;
      background: #fff1e5;
      font-size: 23px;
      margin-bottom: 18px;
    }

    .service-card h3 {
      margin-bottom: 8px;
      font-size: 20px;
    }

    .service-card p {
      color: var(--gray);
      font-size: 14px;
      min-height: 65px;
    }

    .service-meta {
      display: flex;
      justify-content: space-between;
      align-items: center;
      margin-top: 20px;
      padding-top: 16px;
      border-top: 1px solid var(--border);
    }

    .request {
      color: var(--orange-dark);
      font-weight: 800;
      font-size: 13px;
    }

    /* HOW IT WORKS */
    .steps {
      background: var(--black);
      color: white;
    }

    .steps .section-head p {
      color: #bbb;
    }

    .step-grid {
      display: grid;
      grid-template-columns: repeat(4,1fr);
      gap: 18px;
    }

    .step {
      padding: 28px;
      border: 1px solid #333;
      border-radius: 18px;
      background: #1d1d1d;
    }

    .step-number {
      color: var(--orange);
      font-weight: 900;
      font-size: 14px;
      margin-bottom: 15px;
    }

    .step h3 {
      margin-bottom: 10px;
    }

    .step p {
      color: #bbb;
      font-size: 14px;
    }

    /* VERIFICATION */
    .verify-box {
      max-width: 800px;
      margin: auto;
      background: #f8f8f8;
      border: 1px solid var(--border);
      padding: 35px;
      border-radius: 24px;
    }

    .verify-form {
      display: flex;
      gap: 10px;
      margin: 20px 0;
    }

    .verify-form input {
      flex: 1;
      border: 1px solid var(--border);
      border-radius: 10px;
      padding: 14px;
      outline: none;
    }

    .technician {
      background: white;
      border: 1px solid var(--border);
      border-radius: 15px;
      padding: 20px;
      display: none;
    }

    .verified {
      display: inline-block;
      color: var(--success);
      background: #e9f8f0;
      padding: 5px 9px;
      border-radius: 20px;
      font-size: 12px;
      font-weight: 900;
      margin-bottom: 10px;
    }

    /* ABOUT */
    .about-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 50px;
      align-items: center;
    }

    .about-box {
      background: var(--black);
      color: white;
      padding: 35px;
      border-radius: 24px;
    }

    .stats {
      display: grid;
      grid-template-columns: repeat(2,1fr);
      gap: 15px;
      margin-top: 25px;
    }

    .stat {
      padding: 20px;
      border: 1px solid #333;
      border-radius: 15px;
    }

    .stat strong {
      color: var(--orange);
      font-size: 30px;
      display: block;
    }

    /* CTA */
    .cta {
      background: linear-gradient(135deg, var(--orange), #ff9b49);
      color: white;
      text-align: center;
    }

    .cta h2 {
      font-size: clamp(32px, 5vw, 52px);
      line-height: 1.05;
      margin-bottom: 15px;
    }

    .cta p {
      max-width: 650px;
      margin: 0 auto 25px;
    }

    .cta .btn {
      background: white;
      color: var(--black);
    }

    /* FOOTER */
    footer {
      background: #111;
      color: white;
      padding: 55px 0 25px;
    }

    .footer-grid {
      display: grid;
      grid-template-columns: 1.5fr 1fr 1fr;
      gap: 40px;
    }

    footer p,
    footer a {
      color: #aaa;
      font-size: 14px;
    }

    footer h4 {
      margin-bottom: 14px;
    }

    .footer-links {
      display: grid;
      gap: 8px;
    }

    .copyright {
      border-top: 1px solid #2a2a2a;
      margin-top: 40px;
      padding-top: 20px;
      color: #777;
      font-size: 13px;
    }

    /* MODAL */
    .modal {
      display: none;
      position: fixed;
      inset: 0;
      background: rgba(0,0,0,.65);
      z-index: 2000;
      align-items: center;
      justify-content: center;
      padding: 20px;
    }

    .modal.active {
      display: flex;
    }

    .modal-content {
      width: min(600px,100%);
      background: white;
      border-radius: 22px;
      padding: 30px;
      position: relative;
      max-height: 90vh;
      overflow-y: auto;
    }

    .close {
      position: absolute;
      right: 20px;
      top: 15px;
      border: none;
      background: none;
      font-size: 28px;
      cursor: pointer;
    }

    .form-group {
      margin-bottom: 15px;
    }

    .form-group label {
      display: block;
      font-weight: 700;
      margin-bottom: 6px;
      font-size: 13px;
    }

    .form-group input,
    .form-group select,
    .form-group textarea {
      width: 100%;
      padding: 12px;
      border: 1px solid var(--border);
      border-radius: 9px;
      outline: none;
    }

    /* MOBILE */
    @media (max-width: 850px) {
      .nav-links {
        display: none;
      }

      .hero-grid,
      .about-grid {
        grid-template-columns: 1fr;
      }

      .service-grid {
        grid-template-columns: repeat(2,1fr);
      }

      .step-grid {
        grid-template-columns: repeat(2,1fr);
      }

      .footer-grid {
        grid-template-columns: 1fr 1fr;
      }
    }

    @media (max-width: 600px) {
      h1 {
        letter-spacing: -2px;
      }

      .hero {
        padding-top: 55px;
      }

      .service-grid,
      .step-grid,
      .footer-grid {
        grid-template-columns: 1fr;
      }

      .coverage {
        grid-template-columns: 1fr;
      }

      .verify-form {
        flex-direction: column;
      }

      section {
        padding: 60px 0;
      }
    }
  </style>
</head>

<body>

<header>
  <div class="container nav">
    <a href="#" class="logo">
      <!-- Replace logo.png with your official Dewcort logo -->
      <img src="logo.png" alt="Dewcort Engineering Ltd">
      <span>QFix</span>
    </a>

    <nav class="nav-links">
      <a href="#services">Services</a>
      <a href="#how">How it works</a>
      <a href="#verify">Verify Technician</a>
      <a href="#about">About</a>
      <button class="btn btn-primary" onclick="openModal()">Book a Service</button>
    </nav>
  </div>
</header>

<!-- HERO -->
<section class="hero">
  <div class="container hero-grid">

    <div>
      <span class="eyebrow">DEWCORT ENGINEERING LTD</span>

      <h1>
        Professional MEPF services,
        <span>made simple.</span>
      </h1>

      <p>
        Book verified and licensed technicians anywhere in Nigeria.
        From sales and servicing to installation, Dewcort-QFix connects
        you with professional engineering solutions backed by Dewcort Engineering Ltd.
      </p>

      <div class="hero-buttons">
        <button class="btn btn-primary" onclick="openModal()">
          Book a Service →
        </button>

        <a href="#services" class="btn btn-outline">
          Browse Services
        </a>
      </div>
    </div>

    <div class="hero-card">
      <h3>Engineering you can trust.</h3>
      <p>
        Reliable MEPF solutions for homes, businesses, facilities and
        projects across Nigeria.
      </p>

      <div class="coverage">
        <div>
          <strong>36</strong>
          <small>States covered</small>
        </div>

        <div>
          <strong>20+</strong>
          <small>Technicians</small>
        </div>

        <div>
          <strong>100%</strong>
          <small>Verified network</small>
        </div>
      </div>
    </div>

  </div>
</section>

<!-- SERVICES -->
<section id="services">
  <div class="container">

    <div class="section-head">
      <h2>Facility services for every need.</h2>
      <p>
        From equipment sales to servicing and complete installation,
        choose what you need and request a quotation.
      </p>
    </div>

    <div class="filters">
      <button class="filter active" data-filter="all">All</button>
      <button class="filter" data-filter="plumbing">Plumbing</button>
      <button class="filter" data-filter="electrical">Electrical</button>
      <button class="filter" data-filter="hvac">HVAC</button>
      <button class="filter" data-filter="fire">Fire Safety</button>
      <button class="filter" data-filter="solar">Solar / Inverter</button>
      <button class="filter" data-filter="water">Water Treatment</button>
      <button class="filter" data-filter="borehole">Bore-hole</button>
      <button class="filter" data-filter="project">Project Management</button>
      <button class="filter" data-filter="handy">Handy Services</button>
    </div>

    <div class="service-grid">

      <article class="service-card" data-category="plumbing">
        <div class="service-icon">🚰</div>
        <h3>Plumbing</h3>
        <p>
          Installation, leak detection, repairs, water supply systems,
          sanitary fittings and plumbing materials.
        </p>
        <div class="service-meta">
          <span>Sales · Service · Installation</span>
          <a class="request" href="#" onclick="openModal('Plumbing')">Request →</a>
        </div>
      </article>

      <article class="service-card" data-category="electrical">
        <div class="service-icon">⚡</div>
        <h3>Electrical</h3>
        <p>
          Wiring, rewiring, switchboards, sockets, fault diagnosis,
          cables, breakers and electrical safety.
        </p>
        <div class="service-meta">
          <span>Sales · Service · Installation</span>
          <a class="request" href="#" onclick="openModal('Electrical')">Request →</a>
        </div>
      </article>

      <article class="service-card" data-category="hvac">
        <div class="service-icon">❄️</div>
        <h3>Air Conditioning / HVAC</h3>
        <p>
          AC sales, installation, servicing, chemical wash,
          gas top-up and HVAC performance checks.
        </p>
        <div class="service-meta">
          <span>Sales · Service · Installation</span>
          <a class="request" href="#" onclick="openModal('HVAC')">Request →</a>
        </div>
      </article>

      <article class="service-card" data-category="fire">
        <div class="service-icon">🔥</div>
        <h3>Fire Safety</h3>
        <p>
          Fire alarms, extinguishers, detectors, suppression systems,
          inspections, testing and maintenance.
        </p>
        <div class="service-meta">
          <span>Protection · Inspection</span>
          <a class="request" href="#" onclick="openModal('Fire Safety')">Request →</a>
        </div>
      </article>

      <article class="service-card" data-category="solar">
        <div class="service-icon">☀️</div>
        <h3>Solar / Inverter</h3>
        <p>
          Solar panels, inverter systems, batteries, installation,
          commissioning, servicing and load audits.
        </p>
        <div class="service-meta">
          <span>Sales · Service · Installation</span>
          <a class="request" href="#" onclick="openModal('Solar / Inverter')">Request →</a>
        </div>
      </article>

      <article class="service-card" data-category="water">
        <div class="service-icon">💧</div>
        <h3>Water Treatment</h3>
        <p>
          Water quality solutions, treatment systems, filtration,
          installation and maintenance.
        </p>
        <div class="service-meta">
          <span>Sales · Service</span>
          <a class="request" href="#" onclick="openModal('Water Treatment')">Request →</a>
        </div>
      </article>

      <article class="service-card" data-category="borehole">
        <div class="service-icon">🛠️</div>
        <h3>Bore-hole</h3>
        <p>
          Bore-hole drilling, casing, pump installation, accessories,
          servicing and test runs.
        </p>
        <div class="service-meta">
          <span>Installation · Service</span>
          <a class="request" href="#" onclick="openModal('Bore-hole')">Request →</a>
        </div>
      </article>

      <article class="service-card" data-category="project">
        <div class="service-icon">📐</div>
        <h3>Project Management</h3>
        <p>
          Planning, procurement, supervision, quality control,
          progress reporting and commissioning.
        </p>
        <div class="service-meta">
          <span>Consultancy · Delivery</span>
          <a class="request" href="#" onclick="openModal('Project Management')">Request →</a>
        </div>
      </article>

      <article class="service-card" data-category="handy">
        <div class="service-icon">🔧</div>
        <h3>Handy Services</h3>
        <p>
          Painting, POP ceiling, cleaning, fumigation, generator repairs
          and gadget repairs.
        </p>
        <div class="service-meta">
          <span>Multiple Services</span>
          <a class="request" href="#" onclick="openModal('Handy Services')">Request →</a>
        </div>
      </article>

    </div>
  </div>
</section>

<!-- HOW IT WORKS -->
<section class="steps" id="how">
  <div class="container">

    <div class="section-head">
      <h2>Book in four simple steps.</h2>
      <p>
        From selecting your service to receiving your quotation,
        Dewcort-QFix keeps the process simple.
      </p>
    </div>

    <div class="step-grid">

      <div class="step">
        <div class="step-number">STEP 01</div>
        <h3>Browse Services</h3>
        <p>
          Choose plumbing, electrical, HVAC, fire safety, solar,
          bore-hole, project management and more.
        </p>
      </div>

      <div class="step">
        <div class="step-number">STEP 02</div>
        <h3>Book Online</h3>
        <p>
          Tell us what you need, your location and preferred service date.
        </p>
      </div>

      <div class="step">
        <div class="step-number">STEP 03</div>
        <h3>Technician Dispatched</h3>
        <p>
          A verified Dewcort technician is assigned to your request.
        </p>
      </div>

      <div class="step">
        <div class="step-number">STEP 04</div>
        <h3>Get Your Invoice</h3>
        <p>
          Receive a professional quotation/invoice that can be downloaded
          and shared.
        </p>
      </div>

    </di
