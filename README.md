<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Md Riad Ali - Frontend Developer</title>
  <style>
    /* Gradient Background */
    body {
      margin: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background: linear-gradient(135deg, #6a11cb 0%, #2575fc 100%);
      color: #fff;
      min-height: 100vh;
      display: flex;
      flex-direction: column;
      align-items: center;
      padding: 2rem;
    }

    h1 {
      font-size: 3rem;
      font-weight: 900;
      background: linear-gradient(90deg, #f7971e, #ffd200);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      margin-bottom: 0.5rem;
      text-align: center;
      user-select: none;
    }

    .subtitle {
      font-size: 1.5rem;
      font-weight: 600;
      margin-bottom: 2rem;
      text-align: center;
      color: #ffd200cc;
    }

    /* Typing animation container */
    #typing-text {
      font-size: 1.5rem;
      height: 2.2rem; /* reserve space */
      margin-bottom: 3rem;
      font-weight: 600;
      color: #fff;
      text-align: center;
      letter-spacing: 2px;
      user-select: none;
      font-family: 'Courier New', Courier, monospace;
    }

    /* Skill report styles */
    .skills-container {
      max-width: 600px;
      width: 100%;
      background: rgba(255, 255, 255, 0.1);
      border-radius: 15px;
      padding: 2rem;
      box-shadow: 0 8px 32px 0 rgba(0,0,0,0.2);
      backdrop-filter: blur(8px);
      -webkit-backdrop-filter: blur(8px);
    }

    .skill {
      margin-bottom: 1.5rem;
    }

    .skill-label {
      font-weight: 700;
      font-size: 1.1rem;
      margin-bottom: 0.5rem;
      display: flex;
      align-items: center;
      gap: 10px;
    }

    .skill-label span.emoji {
      font-size: 1.4rem;
    }

    /* Gradient bar background */
    .skill-bar-bg {
      background: #333;
      border-radius: 50px;
      height: 22px;
      overflow: hidden;
      box-shadow: inset 0 2px 4px rgba(255,255,255,0.1);
    }

    /* Gradient bar fill with smooth transition */
    .skill-bar-fill {
      height: 100%;
      border-radius: 50px;
      width: 0;
      max-width: 100%;
      transition: width 1.5s ease-in-out;
    }

    /* Colors for each skill */
    .html { background: linear-gradient(90deg, #e44d26, #f16529); }
    .css { background: linear-gradient(90deg, #264de4, #2965f1); }
    .tailwind { background: linear-gradient(90deg, #38b2ac, #319795); }
    .js { background: linear-gradient(90deg, #f7df1e, #f0c419); }
    .react { background: linear-gradient(90deg, #61dafb, #21a1f1); }

    .skill-percent {
      font-weight: 700;
      float: right;
      margin-top: -26px;
      margin-right: 10px;
      color: #fff;
      text-shadow: 0 0 5px rgba(0,0,0,0.6);
      user-select: none;
      font-family: 'Courier New', Courier, monospace;
    }

    /* Footer */
    footer {
      margin-top: 3rem;
      font-size: 1rem;
      color: #ffd200cc;
      user-select: none;
      text-align: center;
    }

    /* Responsive */
    @media (max-width: 640px) {
      h1 {
        font-size: 2.2rem;
      }
      .skills-container {
        padding: 1.5rem;
      }
    }
  </style>
</head>
<body>

  <h1>Md Riad Ali</h1>
  <div class="subtitle">🚀 Frontend Developer | HTML, CSS, Tailwind, JS, React 👨‍💻</div>

  <div id="typing-text"></div>

  <div class="skills-container" aria-label="Skill report">
    <div class="skill">
      <div class="skill-label"><span class="emoji">🟧</span> HTML</div>
      <div class="skill-bar-bg" role="progressbar" aria-valuenow="95" aria-valuemin="0" aria-valuemax="100">
        <div class="skill-bar-fill html" style="width: 0;"></div>
      </div>
      <div class="skill-percent">95%</div>
    </div>

    <div class="skill">
      <div class="skill-label"><span class="emoji">🟦</span> CSS</div>
      <div class="skill-bar-bg" role="progressbar" aria-valuenow="90" aria-valuemin="0" aria-valuemax="100">
        <div class="skill-bar-fill css" style="width: 0;"></div>
      </div>
      <div class="skill-percent">90%</div>
    </div>

    <div class="skill">
      <div class="skill-label"><span class="emoji">🌊</span> Tailwind CSS</div>
      <div class="skill-bar-bg" role="progressbar" aria-valuenow="85" aria-valuemin="0" aria-valuemax="100">
        <div class="skill-bar-fill tailwind" style="width: 0;"></div>
      </div>
      <div class="skill-percent">85%</div>
    </div>

    <div class="skill">
      <div class="skill-label"><span class="emoji">💛</span> JavaScript</div>
      <div class="skill-bar-bg" role="progressbar" aria-valuenow="80" aria-valuemin="0" aria-valuemax="100">
        <div class="skill-bar-fill js" style="width: 0;"></div>
      </div>
      <div class="skill-percent">80%</div>
    </div>

    <div class="skill">
      <div class="skill-label"><span class="emoji">⚛️</span> React</div>
      <div class="skill-bar-bg" role="progressbar" aria-valuenow="75" aria-valuemin="0" aria-valuemax="100">
        <div class="skill-bar-fill react" style="width: 0;"></div>
      </div>
      <div class="skill-percent">75%</div>
    </div>
  </div>

  <footer>
    <p>👋 Thanks for visiting my profile!</p>
  </footer>

  <script>
    // Typing animation - 1 char per second
    const typingText = "Hello, I'm Md Riad Ali 👋 A passionate Frontend Developer!";
    let currentChar = 0;
    const typingElement = document.getElementById('typing-text');

    function type() {
      if (currentChar < typingText.length) {
        typingElement.textContent += typingText.charAt(currentChar);
        currentChar++;
        setTimeout(type, 1000); // 1 second per character
      }
    }
    type();

    // Animate skill bars
    window.onload = () => {
      const skills = [
        { selector: '.html', width: 95 },
        { selector: '.css', width: 90 },
        { selector: '.tailwind', width: 85 },
        { selector: '.js', width: 80 },
        { selector: '.react', width: 75 },
      ];

      skills.forEach(skill => {
        const bar = document.querySelector(skill.selector);
        setTimeout(() => {
          bar.style.width = skill.width + '%';
        }, 1500); // delay to start animation after typing
      });
    }
  </script>
</body>
</html>
