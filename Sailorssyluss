<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>ISS Launch Screen & Blog</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css"/>
  <style>
    /* Launch screen styles */
    #launchScreen {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: rgba(0,0,0,0.8);
      display: flex;
      align-items: center;
      justify-content: center;
      z-index: 9999;
    }
    #launchScreen .box {
      background: #fff;
      padding: 40px;
      border-radius: 12px;
      box-shadow: 0 4px 15px rgba(0,0,0,0.3);
      text-align: center;
      font-family: Arial, sans-serif;
      width: 250px;
      position: relative;
      animation: pulse 1.5s infinite;
    }
    #launchScreen h1 {
      margin: 0;
      font-size: 24px;
      font-weight: bold;
    }
    .loading-text {
      margin-top: 20px;
      font-family: Arial, sans-serif;
      font-size: 16px;
      font-weight: normal;
    }
    .progress-container {
      width: 100%;
      height: 20px;
      background-color: #ddd;
      border-radius: 10px;
      margin-top: 10px;
      overflow: hidden;
    }
    .progress-bar {
      height: 100%;
      width: 0%;
      background-color: #4e54c8;
      transition: width 0.3s ease;
      border-radius: 10px 0 0 10px;
    }
    @keyframes pulse {
      0% { transform: scale(1); }
      50% { transform: scale(1.02); }
      100% { transform: scale(1); }
    }

    /* Main page styles */
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background: pink;
      color: #333;
      scroll-behavior: smooth;
    }
    header {
      background: linear-gradient(to right, #4e54c8, #8f94fb);
      padding: 20px;
      color: white;
      text-align: center;
      animation: fadeIn 1s ease-in;
    }
    nav {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      background: #333;
    }
    nav a {
      color: white;
      padding: 15px;
      text-decoration: none;
      display: inline-block;
    }
    nav a:hover {
      background: #555;
    }
    section {
      padding: 40px 20px;
    }
    /* Gallery styles */
    .gallery {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
    }
    .gallery img {
      width: 100%;
      max-width: 200px;
      margin: 10px;
      border-radius: 8px;
      cursor: pointer;
      transition: transform 0.2s;
    }
    .gallery img:hover {
      transform: scale(1.05);
    }
    /* Blog posts styles */
    .blog-post {
      background: #fff;
      padding: 15px;
      border-radius: 8px;
      margin-bottom: 20px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1);
    }
    .blog-post img {
      width: 100%;
      height: auto;
      border-radius: 8px;
    }
    .blog-post h3 {
      margin-top: 10px;
    }
    .blog-post p {
      margin: 10px 0;
    }
    .read-more {
      align-self: flex-start;
      text-decoration: none;
      color: #4e54c8;
      font-weight: bold;
    }
    .read-more:hover {
      text-decoration: underline;
    }
    /* Skills styles */
    .skills {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
    }
    .skill {
      background: #4e54c8;
      color: #fff;
      padding: 15px;
      margin: 10px;
      border-radius: 8px;
      width: calc(33% - 40px);
      text-align: center;
    }
    /* Testimonials slider styles */
    .testimonials {
      position: relative;
      max-width: 600px;
      margin: 0 auto;
      overflow: hidden;
    }
    .testimonial {
      display: none;
      padding: 20px;
      background: #fff;
      border-radius: 8px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1);
    }
    .testimonial.active {
      display: block;
    }
    /* Life Event styles */
    .life-event {
      background: #fff;
      padding: 20px;
      border-radius: 8px;
      margin-bottom: 20px;
      display: flex;
      flex-direction: column;
      align-items: center;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1);
    }
    .life-event img {
      max-width: 100%;
      height: auto;
      border-radius: 8px;
    }
    .life-event h3 {
      margin-top: 15px;
    }
    .life-event p {
      margin-top: 10px;
      text-align: center;
    }
    /* Newsletter form styles */
    .newsletter {
      max-width: 400px;
      margin: 0 auto;
      background: #fff;
      padding: 20px;
      border-radius: 8px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1);
    }
    /* Map container */
    .map-container {
      width: 100%;
      height: 400px;
      margin-top: 20px;
    }
    /* Footer styles */
    footer {
      background: #333;
      color: #fff;
      text-align: center;
      padding: 20px 10px;
    }
    footer a {
      color: #fff;
      margin: 0 10px;
      text-decoration: none;
    }
    /* WhatsApp button styles */
    .whatsapp {
      position: fixed;
      bottom: 20px;
      right: 20px;
      background: #25D366;
      color: white;
      padding: 15px;
      border-radius: 50%;
      font-size: 24px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.3);
      z-index: 999;
      display: flex;
      align-items: center;
      justify-content: center;
      cursor: pointer;
      transition: background 0.3s;
    }
    .whatsapp:hover {
      background: #1ebe57;
    }
    /* Lightbox styles for images */
    #lightbox {
      display: none;
      position: fixed;
      z-index: 9999;
      top:0;
      left:0;
      width: 100%;
      height: 100%;
      background: rgba(0,0,0,0.8);
      align-items: center;
      justify-content: center;
    }
    #lightbox img {
      max-width: 90%;
      max-height: 80%;
    }
    /* Animate fadeIn */
    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(-20px); }
      to { opacity: 1; transform: translateY(0); }
    }
  </style>
</head>
<body>
  <!-- Launch Screen -->
  <div id="launchScreen">
    <div class="box">
      <h1>ISS BLOG</h1>
      <div class="loading-text">Loading...</div>
      <div class="progress-container">
        <div class="progress-bar" id="progressBar"></div>
      </div>
    </div>
  </div>

  <!-- Main Content -->
  <header>
    <h1>ITZ SÄÏLÖRS SYLÜS / BLOGGER</h1>
    <p>Navigate Ideas, Capture Dreams</p>
  </header>
  <nav>
    <a href="#home">Home</a>
    <a href="#about">About</a>
    <a href="#blog">Blog</a>
    <a href="#gallery">Gallery</a>
    <a href="#lifeevent">Life Event</a>
    <a href="#skills">Skills</a>
    <a href="#testimonials">Testimonials</a>
    <a href="#map">Map</a>
    <a href="#contact">Contact</a>
    <a href="#newsletter">Subscribe</a>
  </nav>

  <!-- Sections -->
  <section id="home">
    <h2>Welcome to My Blog</h2>
    <p>Join me as I explore thoughts, experiences, and digital creativity.</p>
  </section>

  <section id="about">
    <h2>About Me</h2>
    <p>Hi, I’m SÄÏLÖRS SYLÜS — a digital thinker and creator from Eldoret, Kenya. I love sharing knowledge, design ideas, and real-life inspiration with the world.</p>
  </section>

  <section id="lifeevent">
    <h2>My 2023 Life Event</h2>
    <div class="life-event">
      <img src="https://i.imgur.com/your-image-link.jpg" alt="Me sitting outdoors" />
      <h3>My Journey in 2023</h3>
      <p>This year marked a significant milestone in my life as I embraced new challenges and explored new horizons. It was a year of growth, learning, and unforgettable experiences.</p>
    </div>
  </section>

  <section id="gallery">
    <h2>Photo Gallery</h2>
    <div class="gallery">
      <img src="https://images.unsplash.com/photo-1506744038136-46273834b3fb?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Creative Work" />
      <img src="https://images.unsplash.com/photo-1549887534-7c680844a41b?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Design" />
      <img src="https://images.unsplash.com/photo-1519389950473-47ba0277781c?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Nature Inspiration" />
      <img src="https://images.unsplash.com/photo-1496181133206-80ce9b88a853?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Cityscape" />
    </div>
  </section>

  <section id="blog">
    <h2>Recent Blog Posts</h2>
    <!-- Blog Post 1 -->
    <div class="blog-post">
      <img src="https://images.unsplash.com/photo-1506744038136-46273834b3fb?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Creative Work" />
      <h3>Exploring Digital Creativity</h3>
      <p>This post discusses the importance of creativity in the digital age and how to harness it for personal growth.</p>
      <a class="read-more" href="#">Read More</a>
    </div>
    <!-- Blog Post 2 -->
    <div class="blog-post">
      <img src="https://images.unsplash.com/photo-1549887534-7c680844a41b?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Design" />
      <h3>My Journey in Design</h3>
      <p>Sharing my experiences and tips on becoming a better designer, from beginner to professional.</p>
      <a class="read-more" href="#">Read More</a>
    </div>
    <!-- Blog Post 3 -->
    <div class="blog-post">
      <img src="https://images.unsplash.com/photo-1519389950473-47ba0277781c?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Nature Inspiration" />
      <h3>Inspiration from Nature</h3>
      <p>How nature fuels my creative process and ideas, and tips to find inspiration outdoors.</p>
      <a class="read-more" href="#">Read More</a>
    </div>
  </section>

  <section id="skills">
    <h2>My Skills</h2>
    <div class="skills">
      <div class="skill">Web Design</div>
      <div class="skill">Graphic Design</div>
      <div class="skill">Content Creation</div>
      <div class="skill">Digital Marketing</div>
      <div class="skill">Plumbing Engineer</div>
      <div class="skill">Video Editing</div>
    </div>
  </section>

  <section id="testimonials">
    <h2>What People Say</h2>
    <div class="testimonials">
      <div class="testimonial active">
        <p>"SÄÏLÖRS's work is inspiring and innovative. A true creative!"</p>
        <strong>- Client A</strong>
      </div>
      <div class="testimonial">
        <p>"Amazing designer and thinker. Highly recommend!"</p>
        <strong>- Client B</strong>
      </div>
      <div class="testimonial">
        <p>"Brings ideas to life with passion and skill."</p>
        <strong>- Client C</strong>
      </div>
    </div>
    <button onclick="prevTestimonial()">Prev</button>
    <button onclick="nextTestimonial()">Next</button>
  </section>

  <section id="map">
    <h2>My Location</h2>
    <div class="map-container">
      <iframe
        src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3988.496229365912!2d35.275673715127434!3d0.5142839649886397!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x177db4a365e7b7f1%3A0xb2a0a2f4a9b1c7f!2sEldoret%2C%20Kenya!5e0!3m2!1sen!2sus!4v1689271234567"
        allowfullscreen=""
        loading="lazy"
        style="width:100%; height:100%; border:0;"
      ></iframe>
    </div>
  </section>

  <section id="newsletter">
    <h2>Subscribe to My Newsletter</h2>
    <div class="newsletter">
      <form id="newsletterForm">
        <input type="email" placeholder="Your Email" required />
        <button type="submit">Subscribe</button>
      </form>
    </div>
  </section>

  <section id="contact">
    <h2>Contact Me</h2>
    <form id="contactForm">
      <input type="text" placeholder="Your Name" required />
      <input type="email" placeholder="Your Email" required />
      <textarea rows="5" placeholder="Your Message" required></textarea>
    </form>
  </section>

  <!-- WhatsApp Button -->
  <div class="whatsapp" title="Chat on WhatsApp">
    <i class="fab fa-whatsapp"></i>
  </div>

  <!-- Lightbox for Image Viewing -->
  <div id="lightbox">
    <img src="" alt="Enlarged Image" />
  </div>

  <!-- Scripts -->
  <script>
    // Launch Screen Progress
    window.addEventListener('load', () => {
      const progressBar = document.getElementById('progressBar');
      const duration = 30000; // 30 seconds
      const startTime = Date.now();

      const interval = setInterval(() => {
        const elapsed = Date.now() - startTime;
        const progress = Math.min(elapsed / duration, 1);
        progressBar.style.width = (progress * 100) + '%';
        if (progress >= 1) {
          clearInterval(interval);
        }
      }, 300);

      // Remove launch screen after duration
      setTimeout(() => {
        document.getElementById('launchScreen').style.display = 'none';
      }, duration);
    });

    // Testimonials Slider
    let currentTestimonial = 0;
    const testimonials = document.querySelectorAll('.testimonial');

    function showTestimonial(index) {
      testimonials.forEach((t, i) => {
        t.classList.toggle('active', i === index);
      });
    }

    function prevTestimonial() {
      currentTestimonial = (currentTestimonial - 1 + testimonials.length) % testimonials.length;
      showTestimonial(currentTestimonial);
    }

    function nextTestimonial() {
      currentTestimonial = (currentTestimonial + 1) % testimonials.length;
      showTestimonial(currentTestimonial);
    }

    // WhatsApp Button Click (Optional: add link or action)
    document.querySelector('.whatsapp').addEventListener('click', () => {
      window.open('https://wa.me/YOURNUMBER', '_blank');
    });

    // Lightbox for Image Viewing
    document.querySelectorAll('.gallery img').forEach(img => {
      img.addEventListener('click', () => {
        const lightbox = document.getElementById('lightbox');
        const lightboxImg = lightbox.querySelector('img');
        lightboxImg.src = img.src;
        lightbox.style.display = 'flex';
      });
    });

    document.getElementById('lightbox').addEventListener('click', () => {
      document.getElementById('lightbox').style.display = 'none';
    });
  </script>
</body>
</html>
