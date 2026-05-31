
<style>
@import url('https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;600&family=Playfair+Display:wght@700&display=swap');
*{box-sizing:border-box;margin:0;padding:0;}
.pf{font-family:'DM Sans',sans-serif;background:#faf8f5;color:#2c2a27;padding-bottom:2rem;}
.hero{background:#fff;border-bottom:1px solid #ede9e3;padding:2.5rem 1.5rem 2rem;text-align:center;}
.av{width:80px;height:80px;border-radius:50%;background:#EEEDFE;border:2px solid #AFA9EC;display:flex;align-items:center;justify-content:center;font-family:'Playfair Display',serif;font-size:1.5rem;font-weight:700;color:#3C3489;margin:0 auto 1rem;}
.hero h1{font-family:'Playfair Display',serif;font-size:1.7rem;font-weight:700;color:#26215C;margin-bottom:.3rem;}
.hero .sub{font-size:.85rem;color:#888780;letter-spacing:.04em;margin-bottom:1.1rem;}
.chips{display:flex;flex-wrap:wrap;gap:7px;justify-content:center;margin-bottom:1.25rem;}
.chip{padding:4px 13px;border-radius:20px;font-size:.76rem;font-weight:500;}
.chip-p{background:#EEEDFE;color:#3C3489;border:1px solid #CECBF6;}
.chip-t{background:#E1F5EE;color:#085041;border:1px solid #9FE1CB;}
.chip-a{background:#FAEEDA;color:#633806;border:1px solid #FAC775;}
.chip-c{background:#FAECE7;color:#712B13;border:1px solid #F5C4B3;}
.li-btn{display:inline-flex;align-items:center;gap:7px;padding:8px 20px;background:#0077b5;color:#fff;border-radius:20px;font-size:.82rem;font-weight:500;text-decoration:none;border:none;cursor:pointer;}
.sec{padding:1.5rem 1.25rem;border-top:1px solid #ede9e3;}
.sec-title{font-family:'Playfair Display',serif;font-size:1rem;font-weight:700;color:#26215C;margin-bottom:1.1rem;display:flex;align-items:center;gap:8px;}
.sec-title::after{content:'';flex:1;height:1px;background:#ede9e3;}
.about-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(130px,1fr));gap:9px;}
.a-card{background:#fff;border:1px solid #ede9e3;border-radius:12px;padding:.9rem;text-align:center;}
.a-card .ico{font-size:1.3rem;margin-bottom:.4rem;}
.a-card .lbl{font-size:.72rem;color:#888780;margin-bottom:.2rem;}
.a-card .val{font-size:.82rem;font-weight:500;color:#2c2a27;}
.tg{margin-bottom:1.1rem;}
.tg-lbl{font-size:.71rem;color:#B4B2A9;text-transform:uppercase;letter-spacing:.09em;margin-bottom:.5rem;}
.badges{display:flex;flex-wrap:wrap;gap:6px;}
.bd{display:inline-flex;align-items:center;gap:4px;padding:4px 11px;border-radius:7px;font-size:.76rem;font-weight:500;border:1px solid;}
.bd-p{background:#EEEDFE;color:#3C3489;border-color:#CECBF6;}
.bd-t{background:#E1F5EE;color:#085041;border-color:#9FE1CB;}
.bd-b{background:#E6F1FB;color:#0C447C;border-color:#B5D4F4;}
.bd-a{background:#FAEEDA;color:#633806;border-color:#FAC775;}
.bd-g{background:#EAF3DE;color:#27500A;border-color:#C0DD97;}
.bd-c{background:#FAECE7;color:#712B13;border-color:#F5C4B3;}
.bd-pk{background:#FBEAF0;color:#72243E;border-color:#F4C0D1;}
.proj-stack{display:flex;flex-direction:column;gap:11px;}
.proj{background:#fff;border:1px solid #ede9e3;border-radius:14px;padding:1.1rem 1.1rem 1rem;border-left:3px solid;}
.proj.p1{border-left-color:#5DCAA5;}
.proj.p2{border-left-color:#ED93B1;}
.proj.p3{border-left-color:#AFA9EC;}
.proj-head{display:flex;align-items:center;gap:9px;margin-bottom:.5rem;}
.proj-ico{font-size:1.25rem;}
.proj-name{font-weight:600;font-size:.95rem;color:#2c2a27;}
.proj-stack-txt{font-size:.72rem;color:#888780;margin-top:1px;}
.proj-desc{font-size:.8rem;color:#5F5E5A;line-height:1.6;margin-bottom:.75rem;}
.proj-link{display:inline-flex;align-items:center;gap:5px;font-size:.79rem;color:#185FA5;font-weight:500;text-decoration:none;}
.stats-g{display:grid;grid-template-columns:repeat(auto-fit,minmax(120px,1fr));gap:9px;margin-bottom:1rem;}
.stat{background:#fff;border:1px solid #ede9e3;border-radius:12px;padding:.9rem;text-align:center;}
.stat-n{font-family:'Playfair Display',serif;font-size:1.5rem;font-weight:700;color:#534AB7;}
.stat-l{font-size:.72rem;color:#888780;margin-top:3px;}
.gh-imgs{display:flex;flex-direction:column;gap:9px;margin-bottom:1rem;}
.gh-imgs img{width:100%;border-radius:10px;border:1px solid #ede9e3;}
.quote{background:#EEEDFE;border:1px solid #CECBF6;border-radius:12px;padding:1.25rem;text-align:center;font-family:'Playfair Display',serif;font-size:1rem;color:#3C3489;margin-bottom:.9rem;}
.pv{text-align:center;}
.pv img{border-radius:7px;}
</style>

<div class="pf">
  <div class="hero">
    <div class="av">SV</div>
    <h1>Thota Sai Vedha</h1>
    <p class="sub">Data Science Undergraduate &nbsp;·&nbsp; 2023 – 2027</p>
    <div class="chips">
      <span class="chip chip-p">Data Science Student</span>
      <span class="chip chip-t">Python Developer</span>
      <span class="chip chip-a">PySpark Enthusiast</span>
      <span class="chip chip-c">Future Data Scientist</span>
    </div>
    <a class="li-btn" href="https://www.linkedin.com/in/sai-vedha-thota-37788430a" target="_blank">
      <i class="ti ti-brand-linkedin" aria-hidden="true"></i> LinkedIn
    </a>
  </div>

  <div class="sec">
    <div class="sec-title">About me</div>
    <div class="about-grid">
      <div class="a-card"><div class="ico">🎓</div><div class="lbl">Degree</div><div class="val">B.Sc. Data Science</div></div>
      <div class="a-card"><div class="ico">📊</div><div class="lbl">Passion</div><div class="val">ML & Analytics</div></div>
      <div class="a-card"><div class="ico">🌱</div><div class="lbl">Exploring</div><div class="val">Big Data & AI</div></div>
      <div class="a-card"><div class="ico">⚡</div><div class="lbl">Goal</div><div class="val">Data → Insights</div></div>
    </div>
  </div>

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

  <div class="sec">
    <div class="sec-title">Projects</div>
    <div class="proj-stack">
      <div class="proj p1">
        <div class="proj-head">
          <span class="proj-ico">🥗</span>
          <div>
            <div class="proj-name">NutriTrack</div>
            <div class="proj-stack-txt">Python · Scikit-learn · Pandas · NumPy</div>
          </div>
        </div>
        <div class="proj-desc">ML-based system predicting calorie & nutrient values with feature engineering, data visualisation, and a live Streamlit deployment.</div>
        <a class="proj-link" href="https://nutritrackk.streamlit.app/" target="_blank">Live demo <i class="ti ti-arrow-right" aria-hidden="true"></i></a>
      </div>
      <div class="proj p2">
        <div class="proj-head">
          <span class="proj-ico">🛡️</span>
          <div>
            <div class="proj-name">SafeHer</div>
            <div class="proj-stack-txt">GPS · REST APIs · Android</div>
          </div>
        </div>
        <div class="proj-desc">SOS women safety app with live GPS tracking, shake/voice/manual triggers, fake call & siren alerts, and backend emergency contacts.</div>
        <a class="proj-link" href="https://sheshield04.netlify.app/" target="_blank">Live demo <i class="ti ti-arrow-right" aria-hidden="true"></i></a>
      </div>
      <div class="proj p3">
        <div class="proj-head">
          <span class="proj-ico">🎉</span>
          <div>
            <div class="proj-name">Vinayaka Yuvajana Sangam</div>
            <div class="proj-stack-txt">HTML · CSS · JavaScript</div>
          </div>
        </div>
        <div class="proj-desc">Community festival platform with live streaming, location tracking, image gallery, and a chatbot for user engagement.</div>
        <a class="proj-link" href="https://vinayaka-yuvajana-sangam.github.io/VYS/" target="_blank">Live demo <i class="ti ti-arrow-right" aria-hidden="true"></i></a>
      </div>
    </div>
  </div>

  <div class="sec">
    <div class="sec-title">GitHub activity</div>
    <div class="gh-imgs">
      <img src="https://github-readme-stats.vercel.app/api?username=saivedhathota&show_icons=true&theme=default&hide_border=true&bg_color=ffffff&title_color=534AB7&text_color=5F5E5A&icon_color=5DCAA5" alt="GitHub stats" loading="lazy"/>
      <img src="https://github-readme-streak-stats.herokuapp.com/?user=saivedhathota&theme=default&hide_border=true&background=ffffff&stroke=ede9e3&ring=534AB7&fire=D4537E&currStreakLabel=534AB7" alt="GitHub streak" loading="lazy"/>
      <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=saivedhathota&layout=compact&theme=default&hide_border=true&bg_color=ffffff&title_color=534AB7&text_color=5F5E5A" alt="Top languages" loading="lazy"/>
    </div>
    <div class="stats-g">
      <div class="stat"><div class="stat-n">3</div><div class="stat-l">Projects shipped</div></div>
      <div class="stat"><div class="stat-n">5+</div><div class="stat-l">Tech skills</div></div>
      <div class="stat"><div class="stat-n">2027</div><div class="stat-l">Graduation year</div></div>
    </div>
  </div>

  <div class="sec">
    <div class="sec-title">GitHub trophies</div>
    <img src="https://github-profile-trophy.vercel.app/?username=saivedhathota&theme=flat&margin-w=8&no-frame=true&column=4" style="width:100%;border-radius:10px;border:1px solid #ede9e3;" alt="GitHub trophies" loading="lazy"/>
  </div>

  <div class="sec">
    <div class="quote">"Turning Data Into Insights" ✨</div>
    <div class="pv">
      <img src="https://komarev.com/ghpvc/?username=saivedhathota&label=Profile+Views&color=534AB7&style=flat-square" alt="Profile views"/>
    </div>
  </div>
</div>
