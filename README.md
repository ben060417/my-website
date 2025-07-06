# my-website
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Benjamin Min • Landing Page</title>
  <!-- Google Font -->
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
  <style>
    :root {
      --primary: #1e40af;    /* Replace with your primary brand color */
      --secondary: #10b981;  /* Replace with your accent color */
      --text-dark: #1f2937;
      --text-light: #f9fafb;
      --bg-light: #ffffff;
      --bg-dark: #111827;
      --radius: 8px;
    }

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Inter', sans-serif;
    }

    body {
      color: var(--text-dark);
      background: var(--bg-light);
      line-height: 1.6;
    }

    img {
      max-width: 100%;
      display: block;
    }

    /* Header */
    header {
      background: var(--bg-light);
      padding: 1.5rem 5%;
      display: flex;
      align-items: center;
      justify-content: space-between;
      border-bottom: 1px solid #e5e7eb;
    }

    header .logo {
      font-size: 1.25rem;
      font-weight: 700;
      color: var(--primary);
      text-decoration: none;
    }

    nav a {
      margin-left: 2rem;
      text-decoration: none;
      color: var(--text-dark);
      font-weight: 500;
      transition: color 0.2s ease-in-out;
    }

    nav a:hover {
      color: var(--primary);
    }

    /* Hero */
    .hero {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
      align-items: center;
      gap: 2rem;
      padding: 4rem 5%;
      background: linear-gradient(135deg, var(--primary) 0%, var(--secondary) 100%);
      color: var(--text-light);
    }

    .hero h1 {
      font-size: clamp(2rem, 4vw, 3rem);
      margin-bottom: 1rem;
      line-height: 1.2;
    }

    .hero p {
      margin-bottom: 2rem;
      max-width: 32rem;
    }

    .btn {
      display: inline-block;
      background: var(--text-light);
      color: var(--primary);
      padding: 0.75rem 1.5rem;
      border-radius: var(--radius);
      font-weight: 600;
      text-decoration: none;
      transition: background 0.2s ease-in-out, transform 0.2s ease-in-out;
    }

    .btn:hover {
      background: #dbeafe;
      transform: translateY(-2px);
    }

    /* Features */
    .features {
      padding: 4rem 5%;
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
      gap: 2rem;
    }

    .feature-card {
      background: #f3f4f6;
      padding: 2rem;
      border-radius: var(--radius);
      text-align: center;
      transition: transform 0.2s ease-in-out;
    }

    .feature-card:hover {
      transform: translateY(-4px);
    }

    .feature-card h3 {
      margin-top: 1rem;
      margin-bottom: 0.5rem;
      font-size: 1.25rem;
      color: var(--primary);
    }

    /* Testimonials */
    .testimonials {
      background: #f9fafb;
      padding: 4rem 5%;
    }

    .testimonials h2 {
      text-align: center;
      margin-bottom: 2rem;
      font-size: 2rem;
      color: var(--primary);
    }

    .testimonial-list {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 2rem;
    }

    .testimonial {
      background: var(--bg-light);
      padding: 2rem;
      border-radius: var(--radius);
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.05);
    }

    .testimonial p {
      font-style: italic;
      margin-bottom: 1rem;
    }

    .testimonial .author {
      font-weight: 600;
      color: var(--primary);
    }

    /* CTA */
    .cta {
      padding: 4rem 5%;
      text-align: center;
      background: var(--primary);
      color: var(--text-light);
    }

    .cta h2 {
      font-size: 2rem;
      margin-bottom: 1rem;
    }

    .cta a.btn {
      background: var(--secondary);
      color: var(--text-light);
      margin-top: 1rem;
    }

    /* Footer */
    footer {
      background: var(--bg-dark);
      color: var(--text-light);
      text-align: center;
      padding: 1.5rem 5%;
      font-size: 0.875rem;
    }

    /* Responsive tweaks */
    @media (max-width: 640px) {
      nav {
        display: none; /* Simplify for small screens – upgrade later with JS if needed */
      }
      header {
        justify-content: center;
      }
    }
  </style>
</head>
<body>
  <header>
    <a href="#" class="logo">Benjamin&nbsp;Min</a>
    <nav>
      <a href="#features">Features</a>
      <a href="#testimonials">Stories</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <section class="hero">
    <div class="hero-text">
      <h1>Lead the Change. Fund What Works.</h1>
      <p>Back sustainable clean water projects with 100% transparency, measurable impact, and leadership opportunities built for future nonprofit change makers like you.</p>
      <a href="#contact" class="btn">Get Started</a>
    </div>
    <div class="hero-image">
      <img src="hero-image.png" alt="Hero illustration">
    </div>
  </section>

  <section id="features" class="features">
    <div class="feature-card">
      <img src="https://via.placeholder.com/80" alt="Feature icon">
      <h3>Transparent Funding</h3>
      <p>Every dollar you give is tracked and reported, ensuring complete visibility from donation to deployment.</p>
    </div>
    <div class="feature-card">
      <img src="https://via.placeholder.com/80" alt="Feature icon">
      <h3>Sustainable Solutions</h3>
      <p>We invest in long-term clean water systems powered by local innovation and community ownership.</p>
    </div>
    <div class="feature-card">
      <img src="https://via.placeholder.com/80" alt="Feature icon">
      <h3>Future Leaders</h3>
      <p>Join a movement of student changemakers gaining hands-on experience in nonprofit leadership and social impact.</p>
    </div>
  </section>

  <section id="testimonials" class="testimonials">
    <h2>What Students Say</h2>
    <div class="testimonial-list">
      <div class="testimonial">
        <p>“Seeing exactly where my donation went, and the lives it changed, was powerful. This isn’t charity, it’s real impact.”</p>
        <span class="author">- Alex R.</span>
      </div>
      <div class="testimonial">
        <p>“This water initiative gave me my first opportunity to lead a team and manage a real project that mattered.”</p>
        <span class="author">- Maria S.</span>
      </div>
      <div class="testimonial">
        <p>“Their model of transparency and education should be the standard for every nonprofit.”</p>
        <span class="author">- Kevin L.</span>
      </div>
    </div>
  </section>

  <section id="contact" class="cta">
    <h2>Change the World. One Drop. One Leader. One Village at a Time.</h2>
    <p>Make clean water and nonprofit leadership your legacy.</p>
    <a href="#" class="btn">Join the Community</a>
  </section>

  <footer>
    <p>&copy; 2025 Benjamin&nbsp;Min. All rights reserved.</p>
  </footer>
</body>
</html>
