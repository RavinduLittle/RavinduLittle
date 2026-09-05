<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Ravindu Atthanayake — Front-End Developer & UI/UX Designer</title>
  <meta name="description" content="Portfolio of Ravindu Atthanayake — Front-End Developer and UI/UX Designer from Sri Lanka. React, JavaScript, Node.js specialist.">
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800;900&family=JetBrains+Mono:wght@400;500;700&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="style.css">
</head>
<body>

  <!-- Animated Background -->
  <div class="bg-grid" aria-hidden="true"></div>
  <div class="bg-glow bg-glow--1" aria-hidden="true"></div>
  <div class="bg-glow bg-glow--2" aria-hidden="true"></div>
  <div class="bg-glow bg-glow--3" aria-hidden="true"></div>

  <!-- Floating Particles -->
  <canvas id="particles" aria-hidden="true"></canvas>

  <!-- Navigation -->
  <nav class="nav" id="nav">
    <div class="nav__container">
      <a href="#" class="nav__logo">
        <span class="nav__logo-bracket">&lt;</span>RA<span class="nav__logo-bracket"> /&gt;</span>
      </a>
      <ul class="nav__links">
        <li><a href="#home" class="nav__link active" data-section="home">Home</a></li>
        <li><a href="#about" class="nav__link" data-section="about">About</a></li>
        <li><a href="#skills" class="nav__link" data-section="skills">Skills</a></li>
        <li><a href="#contact" class="nav__link" data-section="contact">Contact</a></li>
      </ul>
      <button class="nav__toggle" id="navToggle" aria-label="Toggle navigation menu">
        <span></span><span></span><span></span>
      </button>
    </div>
  </nav>

  <!-- Mobile Menu -->
  <div class="mobile-menu" id="mobileMenu">
    <ul class="mobile-menu__links">
      <li><a href="#home" class="mobile-menu__link" data-section="home">Home</a></li>
      <li><a href="#about" class="mobile-menu__link" data-section="about">About</a></li>
      <li><a href="#skills" class="mobile-menu__link" data-section="skills">Skills</a></li>
      <li><a href="#contact" class="mobile-menu__link" data-section="contact">Contact</a></li>
    </ul>
  </div>

  <!-- Hero Section -->
  <section class="hero" id="home">
    <div class="hero__container">
      <div class="hero__content">
        <div class="hero__greeting reveal-up" style="--delay: 0.1s">
          <span class="hero__wave">👋</span> Hello, I'm
        </div>
        <h1 class="hero__name reveal-up" style="--delay: 0.25s">
          Ravindu
          <span class="hero__name--gradient">Atthanayake</span>
        </h1>
        <div class="hero__roles reveal-up" style="--delay: 0.4s">
          <div class="hero__role-wrapper">
            <span class="hero__role-prefix">I'm a</span>
            <span class="hero__role-text" id="roleText"></span>
            <span class="hero__cursor">|</span>
          </div>
        </div>
        <p class="hero__description reveal-up" style="--delay: 0.55s">
          A passionate front-end developer and UI/UX designer from Sri Lanka 🇱🇰, crafting beautiful digital experiences with clean code and creative design.
        </p>
        <div class="hero__actions reveal-up" style="--delay: 0.7s">
          <a href="#skills" class="btn btn--primary">
            <span>Explore Skills</span>
            <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M7 17l9.2-9.2M17 17V7H7"/></svg>
          </a>
          <a href="#contact" class="btn btn--ghost">
            <span>Get In Touch</span>
          </a>
        </div>
        <div class="hero__stats reveal-up" style="--delay: 0.85s">
          <div class="hero__stat">
            <span class="hero__stat-number" data-target="5">0</span><span class="hero__stat-plus">+</span>
            <span class="hero__stat-label">Languages</span>
          </div>
          <div class="hero__stat-divider"></div>
          <div class="hero__stat">
            <span class="hero__stat-number" data-target="5">0</span><span class="hero__stat-plus">+</span>
            <span class="hero__stat-label">Frameworks</span>
          </div>
          <div class="hero__stat-divider"></div>
          <div class="hero__stat">
            <span class="hero__stat-number" data-target="4">0</span><span class="hero__stat-plus">+</span>
            <span class="hero__stat-label">OS Platforms</span>
          </div>
        </div>
      </div>
      <div class="hero__visual reveal-up" style="--delay: 0.3s">
        <div class="hero__avatar-ring">
          <div class="hero__avatar-ring-glow"></div>
          <div class="hero__avatar-orbit">
            <div class="hero__orbit-dot" style="--i:0"></div>
            <div class="hero__orbit-dot" style="--i:1"></div>
            <div class="hero__orbit-dot" style="--i:2"></div>
            <div class="hero__orbit-dot" style="--i:3"></div>
            <div class="hero__orbit-dot" style="--i:4"></div>
            <div class="hero__orbit-dot" style="--i:5"></div>
          </div>
          <img src="avatar.jpg" alt="Ravindu Atthanayake" class="hero__avatar-img" loading="eager">
        </div>
        <!-- Floating Tech Icons -->
        <div class="hero__float-icon hero__float-icon--1" aria-hidden="true">⚛️</div>
        <div class="hero__float-icon hero__float-icon--2" aria-hidden="true">🔥</div>
        <div class="hero__float-icon hero__float-icon--3" aria-hidden="true">🎨</div>
        <div class="hero__float-icon hero__float-icon--4" aria-hidden="true">💻</div>
      </div>
    </div>
    <div class="hero__scroll-indicator">
      <div class="hero__scroll-mouse">
        <div class="hero__scroll-wheel"></div>
      </div>
      <span>Scroll Down</span>
    </div>
  </section>

  <!-- About Section -->
  <section class="section about" id="about">
    <div class="section__container">
      <div class="section__header reveal-up">
        <span class="section__tag">About Me</span>
        <h2 class="section__title">
          Crafting Digital
          <span class="text-gradient">Experiences</span>
        </h2>
        <p class="section__subtitle">Get to know me and what drives my passion for development</p>
      </div>

      <div class="about__grid">
        <div class="about__card glass-card reveal-up" style="--delay: 0.15s">
          <div class="about__card-icon">🚀</div>
          <h3 class="about__card-title">Front-End Developer</h3>
          <p class="about__card-text">I specialize in building responsive, performant, and accessible web applications using modern frameworks like React, with a focus on clean code and best practices.</p>
        </div>
        <div class="about__card glass-card reveal-up" style="--delay: 0.3s">
          <div class="about__card-icon">🎨</div>
          <h3 class="about__card-title">UI/UX Designer</h3>
          <p class="about__card-text">I create intuitive and visually stunning user interfaces. From wireframes to high-fidelity prototypes, I design experiences that users love.</p>
        </div>
        <div class="about__card glass-card reveal-up" style="--delay: 0.45s">
          <div class="about__card-icon">🌏</div>
          <h3 class="about__card-title">Based in Sri Lanka</h3>
          <p class="about__card-text">Working from the beautiful island of Sri Lanka 🇱🇰, collaborating with clients and teams worldwide to deliver exceptional digital products.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Skills Section -->
  <section class="section skills" id="skills">
    <div class="section__container">
      <div class="section__header reveal-up">
        <span class="section__tag">My Skills</span>
        <h2 class="section__title">
          Technologies &
          <span class="text-gradient">Tools</span>
        </h2>
        <p class="section__subtitle">A curated collection of technologies I work with daily</p>
      </div>

      <!-- Languages -->
      <div class="skills__category reveal-up" style="--delay: 0.1s">
        <h3 class="skills__category-title">
          <span class="skills__category-icon">⌨️</span> Languages
        </h3>
        <div class="skills__grid">
          <div class="skill-card glass-card" data-tilt>
            <div class="skill-card__icon" style="--accent: #E34F26">
              <svg viewBox="0 0 128 128"><path fill="#E34F26" d="M19.037 113.876L9.032 1.661h109.936l-10.016 112.198-45.019 12.48z"/><path fill="#EF652A" d="M64 116.8l36.378-10.086 8.559-95.878H64z"/><path fill="#fff" d="M64 52.455H45.788L44.53 38.361H64V24.599H29.489l.33 3.692 3.382 37.927H64zm0 35.743l-.061.017-15.327-4.14-.979-10.975H33.816l1.928 21.609 28.193 7.826.063-.017z"/><path fill="#EBEBEB" d="M63.952 52.455v13.763h16.947l-1.597 17.849-15.35 4.143v14.319l28.215-7.82.207-2.325 3.234-36.233.335-3.696h-3.708zm0-27.856v13.762h33.244l.276-3.092.628-6.978.329-3.692z"/></svg>
            </div>
            <span class="skill-card__name">HTML5</span>
            <div class="skill-card__glow" style="--accent: #E34F26"></div>
          </div>
          <div class="skill-card glass-card" data-tilt>
            <div class="skill-card__icon" style="--accent: #1572B6">
              <svg viewBox="0 0 128 128"><path fill="#1572B6" d="M18.814 114.123L8.76 1.352h110.48l-10.064 112.754-45.243 12.543z"/><path fill="#33A9DC" d="M64.001 117.062l36.559-10.136 8.601-96.354h-45.16z"/><path fill="#fff" d="M64.001 51.429h18.302l1.264-14.163H64.001V24.208h34.682l-.332 3.711-3.4 38.114h-30.95z"/><path fill="#EBEBEB" d="M64.083 87.349l-.061.018-15.403-4.159-.985-11.031H33.752l1.937 21.717 28.331 7.863.063-.018z"/><path fill="#fff" d="M81.127 64.675l-1.666 18.522-15.426 4.164v14.39l28.354-7.858.208-2.337 2.406-26.881z"/><path fill="#EBEBEB" d="M64.048 24.208v13.058H30.64l-.277-3.108-.631-7.039-.332-2.911zm-.047 27.221v13.058H46.485l-.277-3.108-.631-7.039-.332-2.911z"/></svg>
            </div>
            <span class="skill-card__name">CSS3</span>
            <div class="skill-card__glow" style="--accent: #1572B6"></div>
          </div>
          <div class="skill-card glass-card" data-tilt>
            <div class="skill-card__icon" style="--accent: #F7DF1E">
              <svg viewBox="0 0 128 128"><path fill="#F0DB4F" d="M1.408 1.408h125.184v125.184H1.408z"/><path fill="#323330" d="M116.347 96.736c-.917-5.711-4.641-10.508-15.672-14.981-3.832-1.761-8.104-3.022-9.377-5.926-.452-1.69-.512-2.642-.226-3.665.821-3.32 4.784-4.355 7.925-3.403 2.023.678 3.938 2.237 5.093 4.724 5.402-3.498 5.391-3.475 9.163-5.879-1.381-2.141-2.118-3.129-3.022-4.045-3.249-3.629-7.676-5.498-14.756-5.355l-3.688.477c-3.534.893-6.902 2.748-8.877 5.235-5.926 6.724-4.236 18.492 2.975 23.335 7.104 5.332 17.54 6.545 18.873 11.531 1.297 6.104-4.486 8.08-10.234 7.378-4.236-.881-6.592-3.034-9.139-6.949-4.688 2.713-4.688 2.713-9.508 5.485 1.143 2.499 2.344 3.63 4.26 5.795 9.068 9.198 31.76 8.746 35.83-5.176.142-.39 1.217-3.622.582-8.58zm-46.115-33.236c-2.776-6.249-9.613-12.285-10.765-14.971-1.074-2.51-1.49-5.662-.226-7.853 1.74-3.003 6.105-3.616 9.02-1.892.452 1.69 3.44 4.45 5.106 6.545 2.558-2.285 2.558-2.285 5.402-4.843-1.417-1.464-3.63-3.678-5.629-5.14C70.54 33.14 66.66 32.178 62.76 32.6c-8.104.786-13.288 6.154-14.131 13.327-.309 6.224 2.13 10.87 7.188 15.262 1.951 1.892 9.854 7.949 10.85 12.03.916 3.892-1.069 7.37-5.176 8.294-3.75.738-7.106-.857-9.197-3.64-1.262-1.76-1.83-3.677-2.499-6.09-3.975 1.087-7.95 2.177-11.926 3.271.631 3.642 1.668 5.547 3.559 8.043 8.894 12.054 31.077 11.18 34.936-3.666.166-.643 1.477-3.749.476-8.745-.786-4.497-5.546-8.576-8.59-11.58z"/></svg>
            </div>
            <span class="skill-card__name">JavaScript</span>
            <div class="skill-card__glow" style="--accent: #F7DF1E"></div>
          </div>
          <div class="skill-card glass-card" data-tilt>
            <div class="skill-card__icon" style="--accent: #ED8B00">
              <svg viewBox="0 0 128 128"><path fill="#0074BD" d="M47.617 98.12s-4.767 2.774 3.397 3.71c9.892 1.13 14.947.968 25.845-1.092 0 0 2.871 1.795 6.873 3.351-24.439 10.47-55.308-.607-36.115-5.969zm-2.988-13.665s-5.348 3.959 2.823 4.805c10.567 1.091 18.91 1.18 33.354-1.6 0 0 1.993 2.025 5.132 3.131-29.542 8.64-62.446.68-41.309-6.336z"/><path fill="#EA2D2E" d="M69.802 61.271c6.025 6.935-1.58 13.17-1.58 13.17s15.289-7.891 8.269-17.777c-6.559-9.215-11.587-13.792 15.635-29.58 0 .001-42.731 10.67-22.324 34.187z"/><path fill="#0074BD" d="M102.123 108.229s3.529 2.91-3.888 5.159c-14.102 4.272-58.706 5.56-71.094.171-4.451-1.938 3.899-4.625 6.526-5.192 2.739-.593 4.303-.485 4.303-.485-4.953-3.487-32.013 6.85-13.743 9.815 49.821 8.076 90.817-3.637 77.896-9.468zM49.912 70.294s-22.686 5.389-8.033 7.348c6.188.828 18.518.638 30.011-.326 9.39-.789 18.813-2.474 18.813-2.474s-3.308 1.419-5.704 3.053c-23.042 6.061-67.544 3.238-54.731-2.958 10.832-5.239 19.644-4.643 19.644-4.643zm40.697 22.747c23.421-12.167 12.591-23.86 5.032-22.285-1.848.385-2.677.72-2.677.72s.688-1.079 2-1.543c14.953-5.255 26.451 15.503-4.823 23.725 0-.002.359-.327.468-.617z"/><path fill="#EA2D2E" d="M76.491 1.587S89.459 14.563 63.79 31.551c-20.584 13.644-4.688 21.413-.001 30.29-12-10.848-20.804-20.392-14.896-29.283 8.674-13.042 32.709-19.377 27.598-31.971z"/><path fill="#0074BD" d="M52.214 126.021c22.476 1.437 57-.8 57.817-11.436 0 0-1.571 4.032-18.577 7.231-19.186 3.612-42.854 3.191-56.887.874 0 .001 2.875 2.381 17.647 3.331z"/></svg>
            </div>
            <span class="skill-card__name">Java</span>
            <div class="skill-card__glow" style="--accent: #ED8B00"></div>
          </div>
          <div class="skill-card glass-card" data-tilt>
            <div class="skill-card__icon" style="--accent: #3776AB">
              <svg viewBox="0 0 128 128"><linearGradient id="pyA" x1="12.959" y1="12.039" x2="68.549" y2="68.549" gradientUnits="userSpaceOnUse"><stop offset="0" stop-color="#387EB8"/><stop offset="1" stop-color="#366994"/></linearGradient><path fill="url(#pyA)" d="M63.391 1.988c-4.222.02-8.252.379-11.8 1.007-10.45 1.846-12.346 5.71-12.346 12.837v9.411h24.693v3.137H29.977c-7.176 0-13.46 4.313-15.426 12.521-2.268 9.405-2.368 15.275 0 25.096 1.755 7.311 5.947 12.519 13.124 12.519h8.491V67.234c0-8.151 7.051-15.34 15.426-15.34h24.665c6.866 0 12.346-5.654 12.346-12.548V15.833c0-6.693-5.646-11.72-12.346-12.837-4.244-.706-8.645-1.027-12.866-1.008zM50.037 9.557c2.55 0 4.634 2.117 4.634 4.721 0 2.593-2.083 4.69-4.634 4.69-2.56 0-4.633-2.097-4.633-4.69-.001-2.604 2.073-4.721 4.633-4.721z"/><linearGradient id="pyB" x1="60.799" y1="62.592" x2="120.067" y2="119.084" gradientUnits="userSpaceOnUse"><stop offset="0" stop-color="#FFE052"/><stop offset="1" stop-color="#FFC331"/></linearGradient><path fill="url(#pyB)" d="M91.682 28.38v10.966c0 8.5-7.208 15.655-15.426 15.655H51.591c-6.752 0-12.346 5.783-12.346 12.549v23.515c0 6.691 5.818 10.628 12.346 12.547 7.816 2.297 15.312 2.713 24.665 0 6.216-1.801 12.346-5.423 12.346-12.547v-9.412H63.938v-3.138h37.012c7.176 0 9.852-5.005 12.348-12.519 2.578-7.735 2.467-15.174 0-25.096-1.774-7.145-5.161-12.521-12.348-12.521h-9.268zM77.809 87.927c2.561 0 4.634 2.097 4.634 4.692 0 2.602-2.074 4.719-4.634 4.719-2.55 0-4.633-2.117-4.633-4.719 0-2.595 2.083-4.692 4.633-4.692z"/></svg>
            </div>
            <span class="skill-card__name">Python</span>
            <div class="skill-card__glow" style="--accent: #3776AB"></div>
          </div>
        </div>
      </div>

      <!-- Frameworks -->
      <div class="skills__category reveal-up" style="--delay: 0.25s">
        <h3 class="skills__category-title">
          <span class="skills__category-icon">🛠️</span> Frameworks & Libraries
        </h3>
        <div class="skills__grid">
          <div class="skill-card glass-card" data-tilt>
            <div class="skill-card__icon" style="--accent: #61DAFB">
              <svg viewBox="0 0 128 128"><g fill="#61DAFB"><circle cx="64" cy="64" r="11.4"/><path d="M107.3 45.2c-2.2-.8-4.5-1.6-6.9-2.3.6-2.4 1.1-4.8 1.5-7.1 2.1-13.2-.2-22.5-6.6-26.1-1.9-1.1-4-1.6-6.4-1.6-7 0-15.9 5.2-24.9 13.9-9-8.7-17.9-13.9-24.9-13.9-2.4 0-4.5.5-6.4 1.6-6.4 3.7-8.7 13-6.6 26.1.4 2.3.9 4.7 1.5 7.1-2.4.7-4.7 1.4-6.9 2.3C8.2 50 1.4 56.6 1.4 64s6.9 14 19.3 18.8c2.2.8 4.5 1.6 6.9 2.3-.6 2.4-1.1 4.8-1.5 7.1-2.1 13.2.2 22.5 6.6 26.1 1.9 1.1 4 1.6 6.4 1.6 7.1 0 16-5.2 24.9-13.9 9 8.7 17.9 13.9 24.9 13.9 2.4 0 4.5-.5 6.4-1.6 6.4-3.7 8.7-13 6.6-26.1-.4-2.3-.9-4.7-1.5-7.1 2.4-.7 4.7-1.4 6.9-2.3 12.5-4.8 19.3-11.4 19.3-18.8s-6.8-14-19.3-18.8zM92.5 14.7c4.1 2.4 5.5 9.8 3.8 20.3-.3 2.1-.8 4.3-1.4 6.6-5.2-1.2-10.7-2-16.5-2.5-3.4-4.8-6.9-9.1-10.4-13 7.4-7.3 14.9-12.3 21-12.3 1.3 0 2.5.3 3.5.9zM81.3 74c-1.8 3.2-3.9 6.4-6.1 9.6-3.7.3-7.4.4-11.2.4-3.9 0-7.6-.1-11.2-.4-2.2-3.2-4.2-6.4-6-9.6-1.9-3.3-3.7-6.7-5.3-10 1.6-3.3 3.4-6.7 5.3-10 1.8-3.2 3.9-6.4 6.1-9.6 3.7-.3 7.4-.4 11.2-.4 3.9 0 7.6.1 11.2.4 2.2 3.2 4.2 6.4 6 9.6 1.9 3.3 3.7 6.7 5.3 10-1.7 3.3-3.4 6.6-5.3 10zm8.3-3.3c1.5 3.5 2.7 6.9 3.8 10.3-3.4.8-7 1.4-10.8 1.9 1.2-1.9 2.5-3.9 3.6-6 1.2-2.1 2.3-4.2 3.4-6.2zM64 97.8c-2.4-2.6-4.7-5.4-6.9-8.3 2.3.1 4.6.2 6.9.2 2.3 0 4.6-.1 6.9-.2-2.2 2.9-4.5 5.7-6.9 8.3zm-18.6-15c-3.8-.5-7.4-1.1-10.8-1.9 1.1-3.3 2.3-6.8 3.8-10.3 1.1 2 2.2 4.1 3.4 6.1 1.2 2.2 2.4 4.1 3.6 6.1zm-7-25.5c-1.5-3.5-2.7-6.9-3.8-10.3 3.4-.8 7-1.4 10.8-1.9-1.2 1.9-2.5 3.9-3.6 6-1.2 2.1-2.3 4.2-3.4 6.2zM64 30.2c2.4 2.6 4.7 5.4 6.9 8.3-2.3-.1-4.6-.2-6.9-.2-2.3 0-4.6.1-6.9.2 2.2-2.9 4.5-5.7 6.9-8.3zm22.2 21l-3.6-6c3.8.5 7.4 1.1 10.8 1.9-1.1 3.3-2.3 6.8-3.8 10.3-1.1-2.1-2.2-4.2-3.4-6.2zM31.7 35c-1.7-10.5-.3-17.9 3.8-20.3 1-.6 2.2-.9 3.5-.9 6 0 13.5 4.9 21 12.3-3.5 3.8-7 8.2-10.4 13-5.8.5-11.3 1.4-16.5 2.5-.6-2.3-1-4.5-1.4-6.6zM7 64c0-4.7 5.7-9.7 15.7-13.4 2-.8 4.2-1.5 6.4-2.1 1.6 5 3.6 10.3 6 15.6-2.4 5.3-4.5 10.5-6 15.5C15.3 75.6 7 69.6 7 64zm28.5 49.3c-4.1-2.4-5.5-9.8-3.8-20.3.3-2.1.8-4.3 1.4-6.6 5.2 1.2 10.7 2 16.5 2.5 3.4 4.8 6.9 9.1 10.4 13-7.4 7.3-14.9 12.3-21 12.3-1.3 0-2.5-.3-3.5-.9zM96.3 93c1.7 10.5.3 17.9-3.8 20.3-1 .6-2.2.9-3.5.9-6 0-13.5-4.9-21-12.3 3.5-3.8 7-8.2 10.4-13 5.8-.5 11.3-1.4 16.5-2.5.6 2.3 1 4.5 1.4 6.6zm9-15.6c-2 .8-4.2 1.5-6.4 2.1-1.6-5-3.6-10.3-6-15.6 2.4-5.3 4.5-10.5 6-15.5 13.8 4 22.1 10 22.1 15.6 0 4.7-5.8 9.7-15.7 13.4z"/></g></svg>
            </div>
            <span class="skill-card__name">React</span>
            <div class="skill-card__glow" style="--accent: #61DAFB"></div>
          </div>
          <div class="skill-card glass-card" data-tilt>
            <div class="skill-card__icon" style="--accent: #339933">
              <svg viewBox="0 0 128 128"><path fill="#339933" d="M112.771 30.334L68.674 4.729c-2.781-1.584-6.402-1.584-9.205 0L14.901 30.334C12.031 31.985 10 35.088 10 38.407v51.142c0 3.319 2.084 6.423 4.954 8.083l11.775 6.688c5.628 2.772 7.617 2.772 10.178 2.772 8.333 0 13.093-5.039 13.093-13.828v-50.49c0-.713-.371-1.774-1.071-1.774h-5.623c-.712 0-2.306 1.061-2.306 1.774v50.49c0 3.896-3.524 7.773-10.11 4.48L18.723 91.06c-.424-.23-.723-.693-.723-1.181V38.407c0-.482.555-.966.982-1.213l44.424-25.561c.415-.235 1.025-.235 1.439 0l43.882 25.555c.42.253.272.722.272 1.219v51.142c0 .488.183.963-.232 1.198l-44.086 25.576c-.378.227-.847.227-1.261 0l-11.307-6.749c-.341-.198-.746-.269-1.073-.086-3.146 1.783-3.726 2.02-6.677 3.043-.726.253-1.797.692.41 1.929l14.798 8.754a9.294 9.294 0 004.647 1.246c1.642 0 3.25-.426 4.667-1.246l43.885-25.582c2.87-1.672 4.23-4.764 4.23-8.083V38.407c0-3.319-1.36-6.414-4.229-8.073zM77.91 81.445c-11.726 0-14.309-3.235-15.17-9.066-.1-.628-.633-1.379-1.272-1.379h-5.731c-.71 0-1.279.86-1.279 1.566 0 7.466 4.059 16.512 23.453 16.512 14.039 0 22.088-5.455 22.088-15.109 0-9.572-6.467-12.084-20.082-13.886-13.762-1.819-15.16-2.738-15.16-5.962 0-2.658 1.184-6.203 11.374-6.203 9.105 0 12.461 1.954 13.842 8.091.118.577.645 1.281 1.246 1.281h5.754c.354 0 .692-.286.898-.584.19-.301.297-.696.254-1.09-1.036-12.19-9.045-17.88-21.994-17.88-12.58 0-20.064 5.322-20.064 14.245 0 9.691 7.484 12.369 19.629 13.566 14.528 1.439 15.6 3.586 15.6 6.468 0 5.006-4.024 7.43-13.286 7.43z"/></svg>
            </div>
            <span class="skill-card__name">Node.js</span>
            <div class="skill-card__glow" style="--accent: #339933"></div>
          </div>
          <div class="skill-card glass-card" data-tilt>
            <div class="skill-card__icon" style="--accent: #ffffff">
              <svg viewBox="0 0 128 128"><path fill="#fff" d="M126.67 98.44c-4.56 1.16-7.38.05-9.91-3.75-5.68-8.51-11.95-16.63-18-24.9-.78-1.07-1.59-2.12-2.6-3.45C89 76 81.85 85.2 75.14 94.77c-2.4 3.42-4.92 4.91-9.22 3.71l26.5-36.17-25.7-35.37c4.17-1.26 7.28-.37 9.81 3.4 5.63 8.36 11.63 16.46 17.78 25.07C100.94 46 107.27 36.7 113.82 27.3c2.37-3.4 4.83-4.7 9.01-3.35L98 59.19z"/><path fill="#fff" d="M1.33 61.74c.72-3.61 1.2-7.29 2.2-10.82 6-21.43 30.6-30.34 47.5-17.06C60.93 41.64 63.39 52.62 62.9 65H7.1c-.84 22.21 15.15 35.62 35.53 28.78 7.15-2.4 11.36-8 13.47-15 1.07-3.51 2.93-4.2 6.18-3.17C57.55 93.2 48.25 101 35.72 101.3 20.71 101.65 8.55 92.02 3.89 77.25c-.65-2.06-1.06-4.2-1.59-6.31-.33-1.2-.53-2.44-.78-3.66.2-1.84.2-3.68-.19-5.54zm5.87-3.14h50.43c-.33-16.06-10.33-27.47-24-27.57-15.02-.12-25.78 11.02-26.43 27.57z"/></svg>
            </div>
            <span class="skill-card__name">Express.js</span>
            <div class="skill-card__glow" style="--accent: #ffffff"></div>
          </div>
          <div class="skill-card glass-card" data-tilt>
            <div class="skill-card__icon" style="--accent: #38B2AC">
              <svg viewBox="0 0 128 128"><path d="M64.004 25.602c-17.067 0-27.73 8.53-32 25.597 6.398-8.531 13.867-11.73 22.398-9.597 4.871 1.214 8.352 4.746 12.207 8.66C72.883 56.629 80.145 64 96.004 64c17.066 0 27.73-8.531 32-25.602-6.399 8.536-13.868 11.735-22.399 9.602-4.87-1.215-8.347-4.746-12.207-8.66-6.27-6.367-13.53-13.738-29.394-13.738zM32.004 64c-17.066 0-27.73 8.531-32 25.602C6.402 81.066 13.87 77.867 22.402 80c4.871 1.215 8.352 4.746 12.207 8.66 6.274 6.367 13.536 13.738 29.395 13.738 17.066 0 27.73-8.53 32-25.597-6.399 8.531-13.868 11.73-22.399 9.597-4.87-1.214-8.347-4.746-12.207-8.66C55.128 71.371 47.868 64 32.004 64zm0 0" fill="#38b2ac"/></svg>
            </div>
            <span class="skill-card__name">Tailwind CSS</span>
            <div class="skill-card__glow" style="--accent: #38B2AC"></div>
          </div>
          <div class="skill-card glass-card" data-tilt>
            <div class="skill-card__icon" style="--accent: #7952B3">
              <svg viewBox="0 0 128 128"><path fill="#7952B3" d="M75.701 65.603c-2.334-.768-5.694-.603-10.08-.603H48v23h18.844c2.944 0 5.012-.315 6.203-.535 2.099-.376 3.854-1.104 5.264-1.982 1.409-.878 2.568-2.459 3.477-4.105.908-1.647 1.363-3.652 1.363-6.01 0-3.071-.803-5.49-2.403-7.259-1.6-1.768-3.506-2.762-5.747-3.506zM108.218 0H19.782C8.847 0 0 8.684 0 19.403V108.6C0 119.318 8.847 128 19.782 128h88.436c10.934 0 19.782-8.682 19.782-19.4V19.404C128 8.684 119.153 0 108.218 0zM49.78 84.404H29.73V39.893h20.674c4.237 0 7.305.274 9.202.823 1.898.55 3.538 1.46 4.921 2.733 1.382 1.273 2.392 2.82 3.028 4.64.637 1.82.955 3.895.955 6.223 0 4.757-1.355 8.412-4.067 10.964-2.713 2.551-6.763 3.828-12.153 3.828H48v15.3h1.78v.001zm38.88-.036H68.833V39.893h19.828c4.236 0 7.304.274 9.201.823 1.898.549 3.538 1.46 4.921 2.733 1.383 1.273 2.393 2.82 3.029 4.64.637 1.82.955 3.895.955 6.223 0 4.757-1.355 8.412-4.067 10.964-2.713 2.551-6.763 3.828-12.153 3.828H87.66v15.3h1v-.036z"/></svg>
            </div>
            <span class="skill-card__name">Bootstrap</span>
            <div class="skill-card__glow" style="--accent: #7952B3"></div>
          </div>
        </div>
      </div>

      <!-- Databases -->
      <div class="skills__category reveal-up" style="--delay: 0.4s">
        <h3 class="skills__category-title">
          <span class="skills__category-icon">🗄️</span> Databases & Tools
        </h3>
        <div class="skills__grid">
          <div class="skill-card glass-card" data-tilt>
            <div class="skill-card__icon" style="--accent: #47A248">
              <svg viewBox="0 0 128 128"><path fill-rule="evenodd" clip-rule="evenodd" fill="#439934" d="M90.491 57.282c-.37-4.79-1.896-9.344-4.548-13.134l-.002-.003c-6.28-8.779-18.277-12.108-26.803-11.96-7.187.11-13.538 2.566-17.1 6.87-5.82 7.025-6.216 17.38-1.191 24.788l.29.416c3.45 4.675 8.67 7.753 14.42 8.64h.003c7.23 1.043 14.86-.81 20.39-5.25l.002-.002c4.606-3.706 7.575-8.93 8.545-14.855l-.006-.01v-.5zm0 0"/><path fill-rule="evenodd" clip-rule="evenodd" fill="#45A538" d="M72.31 50.77a43.972 43.972 0 00-8.282-4.592c.252-.343.464-.73.63-1.152l.003-.007a3.7 3.7 0 00.123-2.262 3.654 3.654 0 00-1.105-1.79l-.002-.002c-.873-.773-1.89-.94-2.888-.948h-.052c-.98.01-1.993.167-2.878.879l-.003.002c-.93.78-1.303 1.998-1.133 3.26.114.796.434 1.504.887 2.07a43.33 43.33 0 00-12.552 7.898c-.09-.115-.182-.228-.28-.339a5.16 5.16 0 00-3.2-1.822 5.097 5.097 0 00-3.62.918c-1.188.847-1.923 2.145-2.095 3.602a5.266 5.266 0 001.2 3.945l.116.138c.46.523.997.925 1.578 1.2a37.098 37.098 0 00-3.077 14.067l-.003.004v.002c-.103 4.786.856 9.603 2.895 13.963l.003.008c3.476 7.377 9.782 13.073 17.68 16.118a42.098 42.098 0 0013.39 3.12l.022.003h.002c.707.072 1.418.113 2.131.113.714 0 1.424-.04 2.131-.113h.003l.022-.003a42.003 42.003 0 0013.39-3.12c7.898-3.045 14.203-8.74 17.68-16.118l.003-.008c2.04-4.36 2.998-9.177 2.895-13.963v-.002l-.003-.004a37.098 37.098 0 00-3.077-14.067c.58-.275 1.118-.677 1.578-1.2l.116-.138a5.266 5.266 0 001.2-3.945c-.172-1.457-.907-2.755-2.095-3.602a5.097 5.097 0 00-3.62-.918 5.16 5.16 0 00-3.2 1.822c-.098.11-.19.224-.28.34a43.33 43.33 0 00-12.551-7.9c.453-.565.773-1.273.887-2.069.17-1.262-.203-2.48-1.133-3.26l-.003-.002c-.885-.712-1.897-.868-2.878-.879h-.052c-.997.008-2.015.175-2.888.948l-.002.002a3.654 3.654 0 00-1.105 1.79 3.7 3.7 0 00.124 2.262l.002.007c.166.422.378.81.63 1.152a43.972 43.972 0 00-8.281 4.592z"/><path fill="#FFF" d="M64.39 91.35c-.43 4.23-.59 8.26-.53 12.41.02 2.26.16 4.52.23 6.78.03.72.05 1.44.05 2.16 0 .82-.57 7.56-1.01 7.56s-1.01-6.74-1.01-7.56c0-.72.02-1.44.05-2.16.07-2.26.21-4.52.23-6.78.06-4.15-.1-8.18-.53-12.41-.42-4.16 1.18-4.16 2.47 0z"/></svg>
            </div>
            <span class="skill-card__name">MongoDB</span>
            <div class="skill-card__glow" style="--accent: #47A248"></div>
          </div>
          <div class="skill-card glass-card" data-tilt>
            <div class="skill-card__icon" style="--accent: #FFCA28">
              <svg viewBox="0 0 128 128"><path fill="#FFA000" d="M0 0h128L108.4 112.4 64 128 19.6 112.4z"/><path fill="#F57C00" d="M64 0v128l44.4-15.6L128 0z"/><path fill="#FFCA28" d="M22.3 99l3.7-42H88l-1.8 19.4L64 83.4l-22.2-7-1.6-17.4h44l1.6-18H40.6l-1.6-18h50l1.6-18H22.3z"/><path fill="#FFF" d="M64 99V83.4l22.2-7 1.8-19.4H64v-18h26l-1.6 18-2.2 24.4z"/></svg>
            </div>
            <span class="skill-card__name">Firebase</span>
            <div class="skill-card__glow" style="--accent: #FFCA28"></div>
          </div>
          <div class="skill-card glass-card" data-tilt>
            <div class="skill-card__icon" style="--accent: #FF6C37">
              <svg viewBox="0 0 128 128"><path fill="#FF6C37" d="M74.3 2L64 14.7 53.7 2H0l64 126L128 2zm0 0"/><path fill="#fff" d="M64 14.7L53.7 2H30.5L64 74.4 97.5 2H74.3zm0 0"/></svg>
            </div>
            <span class="skill-card__name">Postman</span>
            <div class="skill-card__glow" style="--accent: #FF6C37"></div>
          </div>
        </div>
      </div>

      <!-- Operating Systems -->
      <div class="skills__category reveal-up" style="--delay: 0.55s">
        <h3 class="skills__category-title">
          <span class="skills__category-icon">💻</span> Operating Systems
        </h3>
        <div class="skills__grid">
          <div class="skill-card glass-card" data-tilt>
            <div class="skill-card__icon" style="--accent: #0078D6">
              <svg viewBox="0 0 128 128"><path fill="#00ADEF" d="M0 12.402l52.636-7.175.022 50.777-52.627.296L0 12.402zm52.614 49.637l.034 50.83L.03 105.78l-.001-43.92 52.585.18zm6.347-57.824L127.952 0v61.74l-68.991.544V4.215zm69.014 58.179l-.023 61.603-69.014-9.726.072-51.975 68.965.098z"/></svg>
            </div>
            <span class="skill-card__name">Windows</span>
            <div class="skill-card__glow" style="--accent: #0078D6"></div>
          </div>
          <div class="skill-card glass-card" data-tilt>
            <div class="skill-card__icon" style="--accent: #E95420">
              <svg viewBox="0 0 128 128"><circle fill="#DD4814" cx="64" cy="64" r="64"/><path fill="#FFF" d="M64 14.41c-27.39 0-49.59 22.2-49.59 49.59S36.61 113.59 64 113.59 113.59 91.39 113.59 64 91.39 14.41 64 14.41zm0 86.12c-20.18 0-36.53-16.35-36.53-36.53S43.82 27.47 64 27.47 100.53 43.82 100.53 64 84.18 100.53 64 100.53z"/><circle fill="#FFF" cx="64" cy="39.87" r="8.55"/><circle fill="#FFF" cx="43.1" cy="75.06" r="8.55"/><circle fill="#FFF" cx="84.9" cy="75.06" r="8.55"/></svg>
            </div>
            <span class="skill-card__name">Ubuntu</span>
            <div class="skill-card__glow" style="--accent: #E95420"></div>
          </div>
          <div class="skill-card glass-card" data-tilt>
            <div class="skill-card__icon" style="--accent: #557C94">
              <svg viewBox="0 0 128 128"><path fill="#557C94" d="M64 2C29.8 2 2 29.8 2 64s27.8 62 62 62 62-27.8 62-62S98.2 2 64 2zm0 6c30.9 0 56 25.1 56 56s-25.1 56-56 56S8 94.9 8 64 33.1 8 64 8z"/><path fill="#557C94" d="M64 22c-23.2 0-42 18.8-42 42s18.8 42 42 42 42-18.8 42-42-18.8-42-42-42zm-2 14h4v16h-4V36zm-16 20h16v4H46v-4zm18 32h-4V72h4v16zm16-16H64v-4h16v4z"/></svg>
            </div>
            <span class="skill-card__name">Kali Linux</span>
            <div class="skill-card__glow" style="--accent: #557C94"></div>
          </div>
          <div class="skill-card glass-card" data-tilt>
            <div class="skill-card__icon" style="--accent: #3DDC84">
              <svg viewBox="0 0 128 128"><path fill="#3DDC84" d="M21.012 91.126c-5.452.001-9.88-4.426-9.882-9.878v-43.27c0-5.453 4.428-9.881 9.88-9.881 5.453.001 9.882 4.429 9.882 9.881v43.27c0 5.452-4.429 9.878-9.88 9.878zm85.978 0c-5.452 0-9.88-4.426-9.88-9.878v-43.27c0-5.453 4.428-9.881 9.88-9.881s9.88 4.429 9.88 9.881v43.27c.002 5.452-4.428 9.878-9.88 9.878zM80.074 23.126L85.31 13.3c.307-.577.085-1.295-.491-1.603-.577-.307-1.294-.084-1.602.492l-5.308 9.958c-4.378-1.98-9.261-3.087-14.398-3.087-5.139 0-10.027 1.107-14.409 3.09L43.789 12.19c-.306-.576-1.024-.799-1.601-.492-.576.308-.799 1.026-.492 1.604l5.236 9.825c-9.393 5.04-15.92 14.16-17.138 24.824h69.417c-1.218-10.663-7.745-19.781-17.137-24.825zM49.779 34.457c-1.539 0-2.788-1.249-2.788-2.788s1.249-2.788 2.788-2.788 2.788 1.249 2.788 2.788-1.249 2.788-2.788 2.788zm28.456 0c-1.539 0-2.788-1.249-2.788-2.788s1.249-2.788 2.788-2.788c1.539 0 2.788 1.249 2.788 2.788s-1.249 2.788-2.788 2.788zM27.221 51.159v42.255c0 3.862 3.137 7 7 7h5.252v14.103c0 5.452 4.428 9.881 9.881 9.881 5.452 0 9.88-4.429 9.88-9.881v-14.103h9.543v14.103c0 5.452 4.429 9.881 9.881 9.881 5.452 0 9.88-4.429 9.88-9.881v-14.103h5.252c3.862 0 7-3.138 7-7V51.159H27.221z"/></svg>
            </div>
            <span class="skill-card__name">Android</span>
            <div class="skill-card__glow" style="--accent: #3DDC84"></div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Contact Section -->
  <section class="section contact" id="contact">
    <div class="section__container">
      <div class="section__header reveal-up">
        <span class="section__tag">Get In Touch</span>
        <h2 class="section__title">
          Let's Build Something
          <span class="text-gradient">Amazing</span>
        </h2>
        <p class="section__subtitle">Have a project in mind? Let's talk about it.</p>
      </div>

      <div class="contact__grid">
        <a href="https://github.com/RavinduLittle" target="_blank" rel="noopener noreferrer" class="contact__card glass-card reveal-up" style="--delay: 0.15s">
          <div class="contact__card-icon" style="--accent: #ffffff">
            <svg viewBox="0 0 24 24" fill="currentColor"><path d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z"/></svg>
          </div>
          <span class="contact__card-label">GitHub</span>
          <span class="contact__card-handle">@RavinduLittle</span>
        </a>
        <div class="contact__card glass-card reveal-up" style="--delay: 0.3s">
          <div class="contact__card-icon" style="--accent: #8b5cf6">
            <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M21 10c0 7-9 13-9 13s-9-6-9-13a9 9 0 0118 0z"/><circle cx="12" cy="10" r="3"/></svg>
          </div>
          <span class="contact__card-label">Location</span>
          <span class="contact__card-handle">Sri Lanka 🇱🇰</span>
        </div>
        <div class="contact__card glass-card reveal-up" style="--delay: 0.45s">
          <div class="contact__card-icon" style="--accent: #06b6d4">
            <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="2" y="3" width="20" height="14" rx="2" ry="2"/><polyline points="22,6 12,13 2,6"/></svg>
          </div>
          <span class="contact__card-label">Email</span>
          <span class="contact__card-handle">Let's Connect</span>
        </div>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer class="footer">
    <div class="footer__container">
      <div class="footer__line"></div>
      <p class="footer__text">
        Designed & Built by <span class="text-gradient">Ravindu Atthanayake</span> © 2026
      </p>
      <p class="footer__sub">Crafted with ❤️ from Sri Lanka</p>
    </div>
  </footer>

  <script src="script.js"></script>
</body>
</html>
