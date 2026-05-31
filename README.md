<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8"/>
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Thota Sai Vedha — Portfolio</title>
  <link href="https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;600&family=Playfair+Display:wght@700&display=swap" rel="stylesheet"/>
  <style>
    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

    body {
      font-family: 'DM Sans', sans-serif;
      background: #faf8f5;
      color: #2c2a27;
      min-height: 100vh;
    }

    .container {
      max-width: 760px;
      margin: 0 auto;
      padding: 0 1.25rem 3rem;
    }

    /* ── HERO ── */
    .hero {
      background: #fff;
      border-bottom: 1px solid #ede9e3;
      padding: 3rem 2rem 2.5rem;
      text-align: center;
      margin-bottom: 0;
    }

    .avatar {
      width: 90px;
      height: 90px;
      border-radius: 50%;
      background: #EEEDFE;
      border: 2px solid #AFA9EC;
      display: flex;
      align-items: center;
      justify-content: center;
      font-family: 'Playfair Display', serif;
      font-size: 1.6rem;
      font-weight: 700;
      color: #3C3489;
      margin: 0 auto 1.2rem;
    }

    .hero h1 {
      font-family: 'Playfair Display', serif;
      font-size: 2rem;
      font-weight: 700;
      color: #26215C;
      margin-bottom: 0.35rem;
    }

    .hero .subtitle {
      font-size: 0.88rem;
      color: #888780;
      letter-spacing: 0.04em;
      margin-bottom: 1.4rem;
    }

    .chips {
      display: flex;
      flex-wrap: wrap;
      gap: 8px;
      justify-content: center;
      margin-bottom: 1.5rem;
    }

    .chip {
      padding: 5px 15px;
      border-radius: 20px;
      font-size: 0.79rem;
      font-weight: 500;
      border: 1px solid;
    }

    .chip-p  { background: #EEEDFE; color: #3C3489; border-color: #CECBF6; }
    .chip-t  { background: #E1F5EE; color: #085041; border-color: #9FE1CB; }
    .chip-a  { background: #FAEEDA; color: #633806; border-color: #FAC775; }
    .chip-c  { background: #FAECE7; color: #712B13; border-color: #F5C4B3; }

    .li-btn {
      display: inline-flex;
      align-items: center;
      gap: 8px;
      padding: 10px 24px;
      background: #0077b5;
      color: #fff;
      border-radius: 24px;
      font-size: 0.85rem;
      font-weight: 500;
      text-decoration: none;
      transition: background 0.2s, transform 0.15s;
    }

    .li-btn:hover { background: #005885; transform: translateY(-1px); }

    .li-icon {
      width: 18px;
      height: 18px;
      fill: white;
    }

    /* ── SECTIONS ── */
    .sec {
      padding: 2rem 0 0;
    }

    .sec-title {
      font-family: 'Playfair Display', serif;
      font-size: 1.1rem;
      font-weight: 700;
      color: #26215C;
      margin-bottom: 1.2rem;
      display: flex;
      align-items: center;
      gap: 10px;
    }

    .sec-title::after {
      content: '';
      flex: 1;
      height: 1px;
      background: #ede9e3;
    }

    /* ── ABOUT GRID ── */
    .about-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(140px, 1fr));
      gap: 10px;
    }

    .a-card {
      background: #fff;
      border: 1px solid #ede9e3;
      border-radius: 12px;
      padding: 1rem;
      text-align: center;
      transition: border-color 0.2s;
    }

    .a-card:hover { border-color: #AFA9EC; }

    .a-card .ico  { font-size: 1.4rem; margin-bottom: 0.45rem; }
    .a-card .lbl  { font-size: 0.72rem; color: #888780; margin-bottom: 0.2rem; }
    .a-card .val  { font-size: 0.84rem; font-weight: 500; color: #2c2a27; }

    /* ── TECH BADGES ── */
    .tg { margin-bottom: 1.2rem; }

    .tg-lbl {
      font-size: 0.72rem;
      color: #B4B2A9;
      text-transform: uppercase;
      letter-spacing: 0.09em;
      margin-bottom: 0.55rem;
    }

    .badges { display: flex; flex-wrap: wrap; gap: 7px; }

    .bd {
      display: inline-flex;
      align-items: center;
      gap: 5px;
      padding: 5px 13px;
      border-radius: 8px;
      font-size: 0.78rem;
      font-weight: 500;
      border: 1px solid;
      transition: transform 0.15s;
    }

    .bd:hover { transform: translateY(-2px); }

    .bd-p  { background: #EEEDFE; color: #3C3489; border-color: #CECBF6; }
    .bd-t  { background: #E1F5EE; color: #085041; border-color: #9FE1CB; }
    .bd-b  { background: #E6F1FB; color: #0C447C; border-color: #B5D4F4; }
    .bd-a  { background: #FAEEDA; color: #633806; border-color: #FAC775; }
    .bd-g  { background: #EAF3DE; color: #27500A; border-color: #C0DD97; }
    .bd-c  { background: #FAECE7; color: #712B13; border-color: #F5C4B3; }

    /* ── PROJECTS ── */
    .proj-stack { display: flex; flex-direction: column; gap: 12px; }

    .proj {
      background: #fff;
      border: 1px solid #ede9e3;
      border-radius: 14px;
      padding: 1.25rem;
      border-left: 3px solid;
      transition: box-shadow 0.2s, transform 0.2s;
    }

    .proj:hover { box-shadow: 0 4px 18px rgba(83,74,183,0.07); transform: translateY(-2px); }

    .proj.p1 { border-left-color: #5DCAA5; }
    .proj.p2 { border-left-color: #ED93B1; }
    .proj.p3 { border-left-color: #AFA9EC; }

    .proj-head { display: flex; align-items: center; gap: 10px; margin-bottom: 0.6rem; }
    .proj-ico  { font-size: 1.35rem; }
    .proj-name { font-weight: 600; font-size: 0.97rem; color: #2c2a27; }
    .proj-tech { font-size: 0.73rem; color: #888780; margin-top: 2px; }

    .proj-desc {
      font-size: 0.83rem;
      color: #5F5E5A;
      line-height: 1.65;
      margin-bottom: 0.8rem;
    }

    .proj-features {
      list-style: none;
      margin-bottom: 0.85rem;
    }

    .proj-features li {
      font-size: 0.79rem;
      color: #5F5E5A;
      padding: 2px 0;
      padding-left: 1rem;
      position: relative;
    }

    .proj-features li::before {
      content: '•';
      position: absolute;
      left: 0;
      color: #AFA9EC;
    }

    .proj-link {
      display: inline-flex;
      align-items: center;
      gap: 5px;
      font-size: 0.8rem;
      color: #185FA5;
      font-weight: 500;
      text-decoration: none;
      transition: gap 0.15s;
    }

    .proj-link:hover { gap: 9px; }

    /* ── GITHUB STATS ── */
    .gh-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 10px;
      margin-bottom: 10px;
    }

    .gh-grid .full { grid-column: 1 / -1; }

    .gh-grid img, .gh-full img {
      width: 100%;
      border-radius: 10px;
      border: 1px solid #ede9e3;
      display: block;
    }

    .stats-g {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(130px, 1fr));
      gap: 10px;
      margin-top: 10px;
    }

    .stat {
      background: #fff;
      border: 1px solid #ede9e3;
      border-radius: 12px;
      padding: 1rem;
      text-align: center;
    }

    .stat-n {
      font-family: 'Playfair Display', serif;
      font-size: 1.6rem;
      font-weight: 700;
      color: #534AB7;
    }

    .stat-l { font-size: 0.73rem; color: #888780; margin-top: 4px; }

    /* ── TROPHIES ── */
    .trophy-img {
      width: 100%;
      border-radius: 10px;
      border: 1px solid #ede9e3;
      display: block;
    }

    /* ── QUOTE ── */
    .quote {
      background: #EEEDFE;
      border: 1px solid #CECBF6;
      border-radius: 12px;
      padding: 1.4rem;
      text-align: center;
      font-family: 'Playfair Display', serif;
      font-size: 1.05rem;
      color: #3C3489;
      margin-bottom: 1rem;
    }

    .pv { text-align: center; }

    /* ── FOOTER ── */
    footer {
      margin-top: 2.5rem;
      padding-top: 1.5rem;
      border-top: 1px solid #ede9e3;
      text-align: center;
      font-size: 0.78rem;
      color: #B4B2A9;
    }

    @media (max-width: 520px) {
      .hero h1 { font-size: 1.5rem; }
      .gh-grid { grid-template-columns: 1fr; }
    }
  </style>
</head>
<body>

  <!-- HERO -->
  <div class="hero">
    <div class="avatar">SV</div>
    <h1>Thota Sai Vedha</h1>
    <p class="subtitle">Data Science Undergraduate &nbsp;·&nbsp; 2023 – 2027</p>
    <div class="chips">
      <span class="chip chip-p">📊 Data Science Student</span>
      <span class="chip chip-t">🐍 Python Developer</span>
      <span class="chip chip-a">⚡ PySpark Enthusiast</span>
      <span class="chip chip-c">🤖 Future Data Scientist</span>
    </div>
    <a class="li-btn" href="https://www.linkedin.com/in/sai-vedha-thota-37788430a" target="_blank">
      <svg class="li-icon" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="M20.447 20.452h-3.554v-5.569c0-1.328-.027-3.037-1.852-3.037-1.853 0-2.136 1.445-2.136 2.939v5.667H9.351V9h3.414v1.561h.046c.477-.9 1.637-1.85 3.37-1.85 3.601 0 4.267 2.37 4.267 5.455v6.286zM5.337 7.433a2.062 2.062 0 01-2.063-2.065 2.064 2.064 0 112.063 2.065zm1.782 13.019H3.555V9h3.564v11.452zM22.225 0H1.771C.792 0 0 .774 0 1.729v20.542C0 23.227.792 24 1.771 24h20.451C23.2 24 24 23.227 24 22.271V1.729C24 .774 23.2 0 22.222 0h.003z"/></svg>
      Connect on LinkedIn
    </a>
  </div>

  <div class="container">

    <!-- ABOUT -->
    <div class="sec">
      <div class="sec-title">About me</div>
      <div class="about-grid">
        <div class="a-card"><div class="ico">🎓</div><div class="lbl">Degree</div><div class="val">B.Sc. Data Science</div></div>
        <div class="a-card"><div class="ico">📊</div><div class="lbl">Passion</div><div class="val">ML & Analytics</div></div>
        <div class="a-card"><div class="ico">🌱</div><div class="lbl">Exploring</div><div class="val">Big Data & AI</div></div>
        <div class="a-card"><div class="ico">⚡</div><div class="lbl">Goal</div><div class="val">Data → Insights</div></div>
      </div>
    </div>

    <!-- TECH STACK -->
    <div class="sec">
      <div class="sec-title">Tech stack</div>

      <div class="tg">
        <div class="tg-lbl">Programming</div>
        <div class="badges">
          <span class="bd bd-b">🐍 Python</span>
          <span class="bd bd-a">JS JavaScript</span>
          <span class="bd bd-t">🗄️ SQL</span>
        </div>
      </div>

      <div class="tg">
        <div class="tg-lbl">Data Science</div>
        <div class="badges">
          <span class="bd bd-p">🐼 Pandas</span>
          <span class="bd bd-t">🔢 NumPy</span>
          <span class="bd bd-g">🤖 Scikit-learn</span>
        </div>
      </div>

      <div class="tg">
        <div class="tg-lbl">Big Data</div>
        <div class="badges">
          <span class="bd bd-a">⚡ Apache Spark</span>
          <span class="bd bd-c">🔥 PySpark</span>
        </div>
      </div>

      <div class="tg">
        <div class="tg-lbl">Web development</div>
        <div class="badges">
          <span class="bd bd-c">🌐 HTML5</span>
          <span class="bd bd-b">🎨 CSS3</span>
        </div>
      </div>
    </div>

    <!-- PROJECTS -->
    <div class="sec">
      <div class="sec-title">Projects</div>
      <div class="proj-stack">

        <div class="proj p1">
          <div class="proj-head">
            <span class="proj-ico">🥗</span>
            <div>
              <div class="proj-name">NutriTrack — Nutritional Estimation System</div>
              <div class="proj-tech">Python · Scikit-learn · Pandas · NumPy · Streamlit</div>
            </div>
          </div>
          <ul class="proj-features">
            <li>Built an ML-based system to predict calorie and nutrient values</li>
            <li>Performed data preprocessing and feature engineering</li>
            <li>Implemented data visualisation for better insights</li>
            <li>Deployed as a live web application</li>
          </ul>
          <a class="proj-link" href="https://nutritrackk.streamlit.app/" target="_blank">Live demo →</a>
        </div>

        <div class="proj p2">
          <div class="proj-head">
            <span class="proj-ico">🛡️</span>
            <div>
              <div class="proj-name">SafeHer — Women Safety App</div>
              <div class="proj-tech">GPS · REST APIs · Android</div>
            </div>
          </div>
          <ul class="proj-features">
            <li>Developed an SOS-based women safety application</li>
            <li>Integrated live GPS tracking for real-time location sharing</li>
            <li>Implemented shake, voice, and manual emergency triggers</li>
            <li>Added fake call and siren alert features</li>
            <li>Managed emergency contacts through backend API integration</li>
          </ul>
          <a class="proj-link" href="https://sheshield04.netlify.app/" target="_blank">Live demo →</a>
        </div>

        <div class="proj p3">
          <div class="proj-head">
            <span class="proj-ico">🎉</span>
            <div>
              <div class="proj-name">Vinayaka Yuvajana Sangam — Festival Platform</div>
              <div class="proj-tech">HTML · CSS · JavaScript</div>
            </div>
          </div>
          <ul class="proj-features">
            <li>Built a community-focused festival web platform</li>
            <li>Integrated live streaming functionality</li>
            <li>Added location tracking and image gallery features</li>
            <li>Developed a chatbot for user assistance and engagement</li>
            <li>Improved accessibility and user experience</li>
          </ul>
          <a class="proj-link" href="https://vinayaka-yuvajana-sangam.github.io/VYS/" target="_blank">Live demo →</a>
        </div>

      </div>
    </div>


  

    <!-- QUOTE + VIEWS -->
    <div class="sec">
      <div class="quote">✨ "Turning Data Into Insights" ✨</div>
      <div class="pv">
        <img src="https://komarev.com/ghpvc/?username=saivedhathota&label=Profile+Views&color=534AB7&style=flat-square" alt="Profile views"/>
      </div>
    </div>

    <footer>
      Thota Sai Vedha &nbsp;·&nbsp; Data Science Undergraduate &nbsp;·&nbsp; 2023–2027
    </footer>

  </div>

</body>
</html>
