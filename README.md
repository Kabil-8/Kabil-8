<div align="center">

<!-- Custom CSS Styling -->
<style>
  /* Gradient Text Animation */
  @keyframes gradient {
    0% { background-position: 0% 50%; }
    50% { background-position: 100% 50%; }
    100% { background-position: 0% 50%; }
  }
  
  /* Glowing Border Animation */
  @keyframes glow {
    0% { box-shadow: 0 0 5px #7F77DD; }
    50% { box-shadow: 0 0 20px #7F77DD, 0 0 30px #F85D7F; }
    100% { box-shadow: 0 0 5px #7F77DD; }
  }
  
  /* Floating Animation */
  @keyframes float {
    0% { transform: translateY(0px); }
    50% { transform: translateY(-10px); }
    100% { transform: translateY(0px); }
  }
  
  /* Shimmer Effect */
  @keyframes shimmer {
    0% { background-position: -200% 0; }
    100% { background-position: 200% 0; }
  }
  
  /* Custom Card Styles */
  .project-card {
    background: linear-gradient(145deg, #1a1b27 0%, #141321 100%);
    border: 1px solid rgba(127, 119, 221, 0.2);
    border-radius: 16px;
    padding: 20px;
    margin: 10px;
    transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
    position: relative;
    overflow: hidden;
  }
  
  .project-card::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 3px;
    background: linear-gradient(90deg, #7F77DD, #F85D7F, #7F77DD);
    background-size: 200% 100%;
    animation: shimmer 3s infinite linear;
  }
  
  .project-card:hover {
    transform: translateY(-5px);
    border-color: #7F77DD;
    box-shadow: 0 10px 40px rgba(127, 119, 221, 0.3);
    animation: glow 2s infinite;
  }
  
  .project-card h3 {
    background: linear-gradient(135deg, #7F77DD 0%, #A9FEF7 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    margin-bottom: 10px;
  }
  
  /* Section Headers */
  .section-header {
    font-size: 2.5em;
    font-weight: 700;
    margin: 40px 0 20px 0;
    background: linear-gradient(45deg, #7F77DD, #A9FEF7, #F85D7F);
    background-size: 200% 200%;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    animation: gradient 4s ease infinite;
    position: relative;
    display: inline-block;
  }
  
  .section-header::after {
    content: '';
    position: absolute;
    bottom: -10px;
    left: 50%;
    transform: translateX(-50%);
    width: 60px;
    height: 3px;
    background: linear-gradient(90deg, #7F77DD, #F85D7F);
    border-radius: 3px;
  }
  
  /* Profile Image Frame */
  .profile-frame {
    width: 150px;
    height: 150px;
    border-radius: 50%;
    padding: 3px;
    background: linear-gradient(135deg, #7F77DD, #F85D7F, #A9FEF7);
    animation: float 3s ease-in-out infinite;
  }
  
  /* Stats Cards Enhancement */
  .stats-container {
    display: flex;
    justify-content: center;
    gap: 20px;
    flex-wrap: wrap;
    margin: 30px 0;
  }
  
  /* Tech Stack Icons Container */
  .tech-stack {
    background: rgba(127, 119, 221, 0.05);
    border-radius: 20px;
    padding: 30px;
    backdrop-filter: blur(10px);
    border: 1px solid rgba(127, 119, 221, 0.1);
  }
  
  /* Connect Buttons */
  .connect-btn {
    display: inline-block;
    padding: 12px 24px;
    margin: 0 10px;
    border-radius: 50px;
    font-weight: 600;
    text-decoration: none;
    transition: all 0.3s ease;
    position: relative;
    overflow: hidden;
  }
  
  .connect-btn::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: linear-gradient(90deg, transparent, rgba(255,255,255,0.2), transparent);
    transition: left 0.5s;
  }
  
  .connect-btn:hover::before {
    left: 100%;
  }
  
  /* Achievement Banner */
  .achievement-banner {
    background: linear-gradient(135deg, rgba(127, 119, 221, 0.1), rgba(248, 93, 127, 0.1));
    border: 1px solid rgba(127, 119, 221, 0.3);
    border-radius: 12px;
    padding: 20px;
    margin: 20px 0;
    backdrop-filter: blur(10px);
  }
  
  /* Divider */
  .custom-divider {
    width: 100%;
    height: 2px;
    background: linear-gradient(90deg, transparent, #7F77DD, #F85D7F, transparent);
    margin: 30px 0;
  }
  
  /* Contribution Calendar Enhancement */
  .contribution-wrapper {
    background: rgba(20, 19, 33, 0.7);
    border-radius: 16px;
    padding: 20px;
    border: 1px solid rgba(127, 119, 221, 0.2);
    backdrop-filter: blur(10px);
  }
  
  /* Status Badge */
  .status-badge {
    display: inline-flex;
    align-items: center;
    padding: 6px 12px;
    background: rgba(127, 119, 221, 0.1);
    border: 1px solid #7F77DD;
    border-radius: 20px;
    font-size: 14px;
    margin: 5px;
  }
  
  .status-dot {
    width: 10px;
    height: 10px;
    border-radius: 50%;
    background: #7F77DD;
    margin-right: 8px;
    animation: glow 2s infinite;
  }
  
  /* Responsive Design */
  @media (max-width: 768px) {
    .section-header {
      font-size: 2em;
    }
    .project-card {
      padding: 15px;
    }
  }
</style>

<!-- Header with Gradient Typography -->
<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=30&duration=3000&pause=1000&color=7F77DD&center=true&vCenter=true&width=435&lines=Hi%2C+I'm+Kabil+%F0%9F%91%8B;Full+Stack+Developer;Building+Scalable+Web+Solutions" alt="Typing SVG" />

<!-- Status Badges -->
<div style="margin: 20px 0;">
  <span class="status-badge">
    <span class="status-dot"></span>
    <span>Active Builder</span>
  </span>
  <span class="status-badge">
    <span class="status-dot" style="background: #F85D7F;"></span>
    <span>21 Repositories</span>
  </span>
  <span class="status-badge">
    <span class="status-dot" style="background: #A9FEF7;"></span>
    <span>Open to Collaborate</span>
  </span>
</div>

![Profile Views](https://komarev.com/ghpvc/?username=Kabil-8&label=Profile%20Views&color=7F77DD&style=flat-square)
[![Open to Work](https://img.shields.io/badge/Available_for_Work-Open-brightgreen?style=flat-square&logo=github)](mailto:kabilk2023@gmail.com)

</div>

<!-- Custom Divider -->
<div class="custom-divider"></div>

<!-- Quick Stats Bar -->
<div class="achievement-banner">
  <div style="display: flex; justify-content: space-around; flex-wrap: wrap;">
    <div style="text-align: center;">
      <h2 style="color: #7F77DD; margin: 0;">🎯 2026</h2>
      <p style="color: #A9FEF7; margin: 5px 0;">Active Year</p>
    </div>
    <div style="text-align: center;">
      <h2 style="color: #F85D7F; margin: 0;">21</h2>
      <p style="color: #A9FEF7; margin: 5px 0;">Repositories</p>
    </div>
    <div style="text-align: center;">
      <h2 style="color: #7F77DD; margin: 0;">5</h2>
      <p style="color: #A9FEF7; margin: 5px 0;">Featured Projects</p>
    </div>
  </div>
</div>

---

## <div class="section-header">🌐 Connect & Collaborate</div>

<div align="center" style="margin: 30px 0;">

<a href="mailto:kabilk2023@gmail.com" class="connect-btn" style="background: #D14836; color: white;">
  <img src="https://img.icons8.com/color/16/000000/gmail-new.png" style="vertical-align: middle; margin-right: 8px;">Email Me
</a>
<a href="https://github.com/Kabil-8" class="connect-btn" style="background: #2b3137; color: white;">
  <img src="https://img.icons8.com/material-outlined/16/ffffff/github.png" style="vertical-align: middle; margin-right: 8px;">GitHub
</a>
<a href="https://linkedin.com/in/your-profile" class="connect-btn" style="background: #0077B5; color: white;">
  <img src="https://img.icons8.com/color/16/000000/linkedin.png" style="vertical-align: middle; margin-right: 8px;">LinkedIn
</a>

</div>

---

## <div class="section-header">📊 2025-2026 Analytics</div>

<div class="contribution-wrapper">
  <p align="center">
    <a href="https://github.com/Kabil-8">
      <img height="180em" src="https://github-readme-stats.vercel.app/api?username=Kabil-8&show_icons=true&theme=radical&hide_border=true&count_private=true&include_all_commits=true&bg_color=141321&title_color=7F77DD&icon_color=F85D7F&text_color=A9FEF7" />
      <img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Kabil-8&layout=compact&theme=radical&hide_border=true&langs_count=8&bg_color=141321&title_color=7F77DD&text_color=A9FEF7" />
    </a>
  </p>
  
  <!-- Activity Graph with Custom Styling -->
  <div style="margin-top: 20px;">
    <a href="https://github.com/Kabil-8">
      <img src="https://github-readme-activity-graph.vercel.app/graph?username=Kabil-8&bg_color=141321&color=A9FEF7&line=7F77DD&point=F85D7F&area=true&hide_border=true" alt="Activity Graph" style="width: 100%;" />
    </a>
  </div>
</div>

<!-- GitHub Streak Stats -->
<p align="center" style="margin-top: 20px;">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=Kabil-8&theme=radical&hide_border=true&background=141321&stroke=7F77DD&ring=F85D7F&fire=F85D7F&currStreakNum=A9FEF7&sideNums=A9FEF7&currStreakLabel=7F77DD&sideLabels=7F77DD&dates=A9FEF7" alt="GitHub Streak" />
</p>

---

## <div class="section-header">🧰 Toolbox & Technologies</div>

<div class="tech-stack">
  <p align="center">
    <img src="https://skillicons.dev/icons?i=js,ts,nodejs,express,react,nextjs,tailwind,mongodb,postgres,java,docker,git&perline=6" />
  </p>
  
  <!-- Language Distribution with Icons -->
  <div style="display: flex; justify-content: center; gap: 30px; margin-top: 20px; flex-wrap: wrap;">
    <div style="display: flex; align-items: center;">
      <img src="https://img.icons8.com/color/24/000000/javascript.png" />
      <span style="color: #A9FEF7; margin-left: 5px;">JavaScript · 45%</span>
    </div>
    <div style="display: flex; align-items: center;">
      <img src="https://img.icons8.com/color/24/000000/typescript.png" />
      <span style="color: #A9FEF7; margin-left: 5px;">TypeScript · 35%</span>
    </div>
    <div style="display: flex; align-items: center;">
      <img src="https://img.icons8.com/color/24/000000/java-coffee-cup-logo.png" />
      <span style="color: #A9FEF7; margin-left: 5px;">Java · 20%</span>
    </div>
  </div>
</div>

---

## <div class="section-header">📌 Featured Work</div>

<!-- Enhanced Project Cards with CSS Classes -->
<div class="project-card">
  <h3 align="center">📊 Finance Dashboard Backend</h3>
  <p align="center">
    <a href="https://github.com/Kabil-8/Finance-Dashboard-Backend">
      <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black" />
      <img src="https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white" />
    </a>
  </p>
  <p align="center" style="color: #A9FEF7;">
    🚀 Robust backend API for financial analytics, budgeting, and real-time data aggregation. Features include transaction tracking, portfolio analysis, and automated reporting.
  </p>
  <div align="center">
    <a href="https://github.com/Kabil-8/Finance-Dashboard-Backend" style="color: #7F77DD; text-decoration: none;">
      ⭐ Star · 🍴 Fork · 👀 Watch
    </a>
  </div>
</div>

<div class="project-card">
  <h3 align="center">🏥 Hospital Management System</h3>
  <p align="center">
    <a href="https://github.com/Kabil-8/Hospital-Management-System">
      <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" />
      <img src="https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black" />
    </a>
  </p>
  <p align="center" style="color: #A9FEF7;">
    💊 Full-stack system for patient registration, appointment scheduling, and inventory management. Real-time bed availability tracking and automated prescription generation.
  </p>
  <div align="center">
    <a href="https://github.com/Kabil-8/Hospital-Management-System" style="color: #7F77DD; text-decoration: none;">
      ⭐ Star · 🍴 Fork · 👀 Watch
    </a>
  </div>
</div>

<div class="project-card">
  <h3 align="center">✍️ The Corporate Blog</h3>
  <p align="center">
    <a href="https://github.com/Kabil-8/The-Corporate-Blog">
      <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black" />
      <img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white" />
    </a>
  </p>
  <p align="center" style="color: #A9FEF7;">
    📝 Clean, SEO-optimized blogging platform with Markdown support and category filtering. Features dynamic routing, image optimization, and integrated analytics dashboard.
  </p>
  <div align="center">
    <a href="https://github.com/Kabil-8/The-Corporate-Blog" style="color: #7F77DD; text-decoration: none;">
      ⭐ Star · 🍴 Fork · 👀 Watch
    </a>
  </div>
</div>

<div class="project-card">
  <h3 align="center">📝 HireFlow Resume Shortlisting</h3>
  <p align="center">
    <a href="https://github.com/Kabil-8/HireFlow-Resume-ShortListing-Platform">
      <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black" />
      <img src="https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white" />
    </a>
  </p>
  <p align="center" style="color: #A9FEF7;">
    🤖 AI-assisted platform to streamline recruitment by parsing and ranking candidate resumes. Includes keyword matching, experience scoring, and automated interview scheduling.
  </p>
  <div align="center">
    <a href="https://github.com/Kabil-8/HireFlow-Resume-ShortListing-Platform" style="color: #7F77DD; text-decoration: none;">
      ⭐ Star · 🍴 Fork · 👀 Watch
    </a>
  </div>
</div>

<div class="project-card">
  <h3 align="center">☕ JavaLearn Platform</h3>
  <p align="center">
    <a href="https://github.com/Kabil-8/JavaLearn-Java-Learning-Platform">
      <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" />
      <img src="https://img.shields.io/badge/Java-E76F00?style=flat-square&logo=openjdk&logoColor=white" />
    </a>
  </p>
  <p align="center" style="color: #A9FEF7;">
    📚 Interactive coding environment and curriculum for learning Java from scratch. Features include live code execution, progress tracking, and community challenges.
  </p>
  <div align="center">
    <a href="https://github.com/Kabil-8/JavaLearn-Java-Learning-Platform" style="color: #7F77DD; text-decoration: none;">
      ⭐ Star · 🍴 Fork · 👀 Watch
    </a>
  </div>
</div>

---

## <div class="section-header">🏆 Achievements & Trophies</div>

<p align="center">
  <img src="https://github-profile-trophy.vercel.app/?username=Kabil-8&theme=radical&no-frame=true&no-bg=false&margin-w=4&row=1&column=7" alt="GitHub Trophies" />
</p>

<!-- Achievement Badges -->
<div class="achievement-banner">
  <div style="display: flex; justify-content: center; gap: 20px; flex-wrap: wrap;">
    <img src="https://img.shields.io/badge/21-Repositories-blue?style=for-the-badge&logo=github" />
    <img src="https://img.shields.io/badge/2026-Active%20Year-purple?style=for-the-badge&logo=github" />
    <img src="https://img.shields.io/badge/Full%20Stack-Developer-orange?style=for-the-badge&logo=devdotto" />
  </div>
</div>

---

<!-- Animated Footer -->
<div class="custom-divider"></div>

<div align="center" style="margin: 40px 0;">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=16&duration=3000&pause=1000&color=7F77DD&center=true&vCenter=true&width=435&lines=Thanks+for+visiting!+%F0%9F%99%8F;Let's+build+something+amazing!+%F0%9F%92%AA;Open+to+collaboration+%F0%9F%A4%9D" alt="Footer Typing SVG" />
  
  <br>
  
  <div style="margin-top: 20px;">
    <img src="https://raw.githubusercontent.com/platane/snk/output/github-contribution-grid-snake-dark.svg" alt="Snake Animation" style="max-width: 100%;" />
  </div>
  
  <p style="color: #A9FEF7; margin-top: 30px; font-size: 14px;">
    🚀 Built with <span style="color: #F85D7F;">❤️</span> by <strong>Kabil</strong> · © 2026 · Last active: April 15, 2026
  </p>
</div>
