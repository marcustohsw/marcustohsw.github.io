---
permalink: /
title: "Home"
redirect_from:
  - /about/
---

Hi, I'm Marcus 👋!
I love building things that make life a little better.

<div class="home-actions">
  <a class="btn btn--primary" href="{{ '/resume/' | relative_url }}">View Resume</a>
</div>

### 💻 Background

I am currently in my final year of <a href="https://www.sutd.edu.sg/istd">B.Eng in Computer Science &amp; Design (CSD)</a> at the <a href="https://www.sutd.edu.sg/">Singapore University of Technology and Design</a>.

<div class="about-terminal" id="about-terminal">
  <div class="terminal-header">
    <div class="terminal-buttons">
      <span class="terminal-dot"></span>
      <span class="terminal-dot"></span>
      <span class="terminal-dot"></span>
    </div>

    <div class="terminal-title">
      marcus@portfolio — ~/about
    </div>
  </div>

  <div class="terminal-body">
    <div class="terminal-line">
      <span class="terminal-prompt">marcus@portfolio:~$</span>
      <span id="command-whoami"></span>
    </div>

    <div class="terminal-output terminal-hidden" id="whoami-output">
      When I'm not coding, you'll usually find me tinkering with software,
      hardware, or some unnecessarily complicated solution to an everyday
      problem. I'm particularly interested in areas where software meets the
      physical world.
    </div>

    <div class="terminal-line terminal-hidden" id="interests-command-line">
      <span class="terminal-prompt">marcus@portfolio:~$</span>
      <span id="command-interests"></span>
    </div>

    <div class="terminal-interests terminal-hidden" id="interests-list">

      <div class="interest-item">
        <div class="interest-main">
          <span class="interest-number">01</span>
          <span class="interest-icon">🤖</span>
          <span class="interest-name">Artificial Intelligence</span>
        </div>
        <div class="interest-details">
          Machine Learning · Computer Vision
        </div>
      </div>

      <div class="interest-item">
        <div class="interest-main">
          <span class="interest-number">02</span>
          <span class="interest-icon">💻</span>
          <span class="interest-name">Software Engineering</span>
        </div>
        <div class="interest-details">
          Python · Java · C++ · Git
        </div>
      </div>

      <div class="interest-item">
        <div class="interest-main">
          <span class="interest-number">03</span>
          <span class="interest-icon">📱</span>
          <span class="interest-name">Application Development</span>
        </div>
        <div class="interest-details">
          Android Applications (Java)
        </div>
      </div>

      <div class="interest-item">
        <div class="interest-main">
          <span class="interest-number">04</span>
          <span class="interest-icon">🦾</span>
          <span class="interest-name">Robotics</span>
        </div>
        <div class="interest-details">
          ROS 2 · Computer Vision on Robots
        </div>
      </div>

      <div class="interest-item">
        <div class="interest-main">
          <span class="interest-number">05</span>
          <span class="interest-icon">🏠</span>
          <span class="interest-name">Internet of Things</span>
        </div>
        <div class="interest-details">
          Smart Home · Networking
        </div>
      </div>

      <div class="interest-item">
        <div class="interest-main">
          <span class="interest-number">06</span>
          <span class="interest-icon">📊</span>
          <span class="interest-name">Data Analytics</span>
        </div>
        <div class="interest-details">
          Data Visualisation · Data Processing
        </div>
      </div>

    </div>

    <div class="terminal-line terminal-hidden" id="final-command-line">
      <span class="terminal-prompt">marcus@portfolio:~$</span>
      <span class="terminal-cursor">█</span>
    </div>

    <div class="terminal-help terminal-hidden" id="terminal-help">
      Type
      <span class="terminal-command-hint">help</span>
      and press Enter.
    </div>

    <div class="terminal-interactive terminal-hidden" id="interactive-terminal">
      <div id="terminal-history"></div>

      <div class="terminal-input-line">
        <span class="terminal-prompt">marcus@portfolio:~$</span>

        <input
          type="text"
          id="terminal-input"
          class="terminal-input"
          autocomplete="off"
          autocapitalize="off"
          spellcheck="false"
          aria-label="Terminal command"
        >
      </div>
    </div>
  </div>
</div>

<!-- Featured Projects Section -->

<section class="home-currently" aria-labelledby="home-currently-title">
  <h3 id="home-currently-title">🌱 Currently Working On</h3>
  <!-- Update this short note as your current work changes. -->
  <p>Building an app to track my snacks and their expiry dates. Follow the <a href="{{ '/projects/snackapp/' | relative_url }}">Snack App project</a>.</p>
</section>

<section class="home-projects" aria-labelledby="home-projects-title">
  <h3 id="home-projects-title">🛠️ Featured Projects</h3>
  <div class="home-project-grid">
    <a class="home-project-card" href="{{ '/projects/computer-vision/' | relative_url }}">
      <img src="{{ '/assets/images/project-vision-placeholder.svg' | relative_url }}" alt="" width="640" height="400" loading="lazy">
      <span class="home-project-overlay">
        <span class="home-project-title">Object Detection &amp; Classification</span>
        <span class="home-project-more">View Project <span aria-hidden="true">&rarr;</span></span>
      </span>
    </a>
    <a class="home-project-card" href="{{ '/projects/robot-interface/' | relative_url }}">
      <img src="{{ '/assets/images/project-robot-placeholder.svg' | relative_url }}" alt="" width="640" height="400" loading="lazy">
      <span class="home-project-overlay">
        <span class="home-project-title">Robot User Interface</span>
        <span class="home-project-more">View Project <span aria-hidden="true">&rarr;</span></span>
      </span>
    </a>
  </div>
</section>

<style>
.home-actions { display: flex; flex-wrap: wrap; gap: 0.75rem; margin: 1.25rem 0 2rem; }
.home-actions .btn { margin: 0; }
.home-actions a:focus-visible, .home-currently a:focus-visible { outline: 3px solid #287b91; outline-offset: 4px; }
.home-currently { margin: 2rem 0; }
.home-currently p { padding-left: 1rem; border-left: 3px solid #287b91; }
.home-projects { margin: 2rem 0; }
.home-project-grid { display: grid; grid-template-columns: repeat(2, minmax(0, 1fr)); gap: 1rem; }
.home-project-grid .home-project-card { position: relative; display: block; overflow: hidden; aspect-ratio: 8 / 5; border: 1px solid #344753; border-radius: 10px; background: #14232f; color: #fff; text-decoration: none; transition: box-shadow 220ms ease, border-color 220ms ease; }
.home-project-card img { display: block; width: 100%; height: 100%; object-fit: cover; transition: transform 300ms ease; }
.home-project-overlay { position: absolute; inset: 0; display: flex; flex-direction: column; justify-content: flex-end; gap: 0.4rem; padding: 1.1rem; background: linear-gradient(transparent 15%, rgba(5, 12, 20, 0.95)); }
.home-project-title { max-width: 26ch; font-size: 0.9em; font-weight: 700; line-height: 1.35; }
.home-project-card:hover, .home-project-card:focus-visible { border-color: #58a6ff; box-shadow: 0 8px 24px rgba(13, 17, 23, 0.2); }
.home-project-card:hover img, .home-project-card:focus-visible img { transform: scale(1.06); }
.home-project-card:focus-visible { outline: 3px solid #287b91; outline-offset: 4px; }
.home-project-more { font-size: 0.7em; color: #b8e4ff; }
@media (hover: hover) and (pointer: fine) {
  .home-project-more { opacity: 0; transform: translateY(5px); transition: opacity 220ms ease, transform 220ms ease; }
  .home-project-card:hover .home-project-more, .home-project-card:focus-visible .home-project-more { opacity: 1; transform: translateY(0); }
}
@media (prefers-reduced-motion: reduce) {
  .home-project-card, .home-project-card img, .home-project-more { transition: none !important; transform: none !important; }
}
@media (max-width: 600px) {
  .home-project-grid { grid-template-columns: 1fr; }
}

.about-terminal {
  width: 100%;
  margin: 2rem 0;
  overflow: hidden;

  border: 1px solid #2a3038;
  border-radius: 10px;

  background: #0d1117;
  color: #f0f6fc;

  font-family:
    "SFMono-Regular",
    Consolas,
    "Liberation Mono",
    Menlo,
    monospace;

  font-size: 0.92rem;
  line-height: 1.7;

  box-shadow:
    0 8px 30px rgba(0, 0, 0, 0.12);

  transition:
    transform 0.3s ease,
    box-shadow 0.3s ease;
}

.about-terminal:hover {
  transform: translateY(-2px);

  box-shadow:
    0 12px 36px rgba(0, 0, 0, 0.16);
}


/* Header */

.terminal-header {
  position: relative;

  display: flex;
  align-items: center;
  justify-content: center;

  min-height: 42px;
  padding: 0 1rem;

  border-bottom: 1px solid #252b33;
  background: #161b22;
}

.terminal-buttons {
  position: absolute;
  left: 14px;

  display: flex;
  gap: 7px;
}

.terminal-dot {
  width: 11px;
  height: 11px;

  border-radius: 50%;
  background: #484f58;
}

.terminal-title {
  color: #8b949e;
  font-size: 0.78rem;

  user-select: none;
}


/* Main terminal */

.terminal-body {
  padding: 1.25rem 1.4rem 1.4rem;
}

.terminal-line {
  display: flex;
  flex-wrap: wrap;
  gap: 0.6rem;

  margin-bottom: 0.55rem;
}

.terminal-prompt {
  color: #58a6ff;
  font-weight: 600;
  white-space: nowrap;
}

.terminal-output {
  max-width: 950px;

  margin:
    0.35rem 0
    1.35rem 0;

  color: #c9d1d9;
}


/* Interests */

.terminal-interests {
  margin:
    0.5rem 0
    1.4rem;
}

.interest-item {
  position: relative;

  max-width: 850px;

  padding:
    0.42rem 0.7rem;

  margin-left: -0.7rem;

  border-radius: 6px;

  opacity: 0;
  transform: translateY(8px);

  transition:
    opacity 0.35s ease,
    transform 0.35s ease,
    background 0.2s ease;
}

.interest-item.interest-visible {
  opacity: 1;
  transform: translateY(0);
}

.interest-item:hover {
  background: rgba(255, 255, 255, 0.045);
}

.interest-main {
  display: grid;

  grid-template-columns:
    2rem
    2rem
    minmax(0, 1fr);

  align-items: center;

  color: #f0f6fc;
}

.interest-number {
  color: #6e7681;
}

.interest-icon {
  font-size: 1rem;
}

.interest-name {
  position: relative;
  width: fit-content;
}

.interest-item:hover .interest-name::before {
  content: ">";

  position: absolute;
  left: -1.1rem;

  color: #7ee787;
}

.interest-details {
  max-height: 0;

  margin-left: 4rem;

  overflow: hidden;

  color: #8b949e;
  font-size: 0.82rem;

  opacity: 0;
  transform: translateY(-3px);

  transition:
    max-height 0.25s ease,
    opacity 0.25s ease,
    transform 0.25s ease;
}

.interest-item:hover .interest-details {
  max-height: 40px;

  opacity: 1;
  transform: translateY(0);
}


/* Cursor */

.terminal-cursor {
  color: #f0f6fc;

  animation:
    terminal-blink 1s steps(1) infinite;
}

@keyframes terminal-blink {
  0%,
  50% {
    opacity: 1;
  }

  51%,
  100% {
    opacity: 0;
  }
}


/* Help */

.terminal-help {
  margin-top: 0.6rem;

  color: #6e7681;
  font-size: 0.78rem;
}

.terminal-command-hint {
  color: #79c0ff;
}


/* Interactive terminal */

.terminal-interactive {
  margin-top: 1rem;
}

.terminal-input-line {
  display: flex;
  gap: 0.6rem;
}

.terminal-input {
  flex: 1;

  min-width: 0;

  border: 0;
  outline: none;

  background: transparent;
  color: #f0f6fc;

  font: inherit;

  caret-color: #f0f6fc;
}

.history-command {
  display: flex;
  gap: 0.6rem;

  margin-top: 0.4rem;
}

.history-output {
  margin:
    0.25rem 0
    0.75rem;

  color: #c9d1d9;

  white-space: pre-line;
}

.history-error {
  color: #ff7b72;
}

.history-link {
  color: #79c0ff;

  text-decoration: none;
}

.history-link:hover {
  text-decoration: underline;
}


/* Hidden */

.terminal-hidden {
  display: none;
}


/* Mobile */

@media (max-width: 700px) {
  .about-terminal {
    font-size: 0.8rem;
  }

  .terminal-body {
    padding: 1rem;
  }

  .terminal-title {
    max-width: 60%;

    overflow: hidden;
    text-overflow: ellipsis;
    white-space: nowrap;
  }

  .terminal-output {
    line-height: 1.65;
  }

  .interest-main {
    grid-template-columns:
      1.7rem
      1.7rem
      1fr;
  }

  .interest-details {
    margin-left: 3.4rem;
  }
}


@media (hover: none) {
  .interest-details { max-height: none; opacity: 1; transform: none; }
}

/* Accessibility */

@media (prefers-reduced-motion: reduce) {
  .about-terminal,
  .interest-item,
  .interest-details,
  .terminal-cursor {
    animation: none !important;
    transition: none !important;
  }
}
</style>

<script>
document.addEventListener("DOMContentLoaded", function () {

  const terminal = document.getElementById("about-terminal");

  const commandWhoami =
    document.getElementById("command-whoami");

  const whoamiOutput =
    document.getElementById("whoami-output");

  const interestsCommandLine =
    document.getElementById("interests-command-line");

  const commandInterests =
    document.getElementById("command-interests");

  const interestsList =
    document.getElementById("interests-list");

  const finalCommandLine =
    document.getElementById("final-command-line");

  const terminalHelp =
    document.getElementById("terminal-help");

  const interactiveTerminal =
    document.getElementById("interactive-terminal");

  const terminalInput =
    document.getElementById("terminal-input");

  const terminalHistory =
    document.getElementById("terminal-history");

  const reducedMotion = window.matchMedia("(prefers-reduced-motion: reduce)").matches;
  let animationStarted = false;


  /* -------------------------
     Typing function
  ------------------------- */

  function typeText(
    element,
    text,
    speed = 60
  ) {

    if (reducedMotion) {
      element.textContent = text;
      return Promise.resolve();
    }

    return new Promise((resolve) => {

      let index = 0;

      const interval =
        setInterval(() => {

          element.textContent =
            text.substring(
              0,
              index + 1
            );

          index++;

          if (
            index >= text.length
          ) {

            clearInterval(
              interval
            );

            resolve();
          }

        }, speed);

    });
  }


  /* -------------------------
     Delay helper
  ------------------------- */

  function delay(ms) {
    if (reducedMotion) return Promise.resolve();

    return new Promise(
      resolve =>
        setTimeout(
          resolve,
          ms
        )
    );

  }


  /* -------------------------
     Main intro animation
  ------------------------- */

  async function startTerminal() {

    if (animationStarted) {
      return;
    }

    animationStarted = true;


    await typeText(
      commandWhoami,
      "whoami",
      75
    );


    await delay(300);


    whoamiOutput
      .classList
      .remove(
        "terminal-hidden"
      );


    await delay(650);


    interestsCommandLine
      .classList
      .remove(
        "terminal-hidden"
      );


    await typeText(
      commandInterests,
      "interests --list",
      55
    );


    await delay(300);


    interestsList
      .classList
      .remove(
        "terminal-hidden"
      );


    const interests =
      interestsList
        .querySelectorAll(
          ".interest-item"
        );


    for (
      let i = 0;
      i < interests.length;
      i++
    ) {

      await delay(110);

      interests[i]
        .classList
        .add(
          "interest-visible"
        );
    }


    await delay(400);


    finalCommandLine
      .classList
      .remove(
        "terminal-hidden"
      );


    terminalHelp
      .classList
      .remove(
        "terminal-hidden"
      );


    interactiveTerminal
      .classList
      .remove(
        "terminal-hidden"
      );

  }


  /* -------------------------
     Start on scroll
  ------------------------- */

  if (
    "IntersectionObserver"
    in window
  ) {

    const observer =
      new IntersectionObserver(
        function (entries) {

          entries.forEach(
            function (entry) {

              if (
                entry.isIntersecting
              ) {

                startTerminal();

                observer.disconnect();
              }

            }
          );

        },
        {
          threshold: 0.25
        }
      );


    observer.observe(
      terminal
    );

  } else {

    startTerminal();

  }


  /* -------------------------
     Terminal commands
  ------------------------- */

  const commands = {

    help: `
Available commands:

  about       |     Who am I?
  interests   |     Things I enjoy working on
  skills      |     Technologies I work with
  projects    |     View my projects
  contact     |     Where to find me
  clear       |     Clear the terminal
`,

    about: `
I'm interested in building useful systems at the intersection
of software, artificial intelligence, hardware and the physical world.
`,

    interests: `
01  🤖  Artificial Intelligence
02  💻  Software Engineering
03  📱  Application Development
04  🦾  Robotics
05  🏠  Internet of Things
06  📊  Data Analytics
`,

    skills: `
AI / Vision
  Python · PyTorch · OpenCV · OpenVINO

Software
  Python · Java · C++ · Git

Applications
  Flutter · Android

Robotics
  ROS · Computer Vision

Systems
  Linux · Networking · IoT
`,

    contact: `
Find me through the LinkedIn, GitHub, and email links in my profile.
`
  };


  /* -------------------------
     Add history item
  ------------------------- */

  function addHistory(
    command,
    output,
    isError = false
  ) {

    const commandElement =
      document.createElement(
        "div"
      );

    commandElement.className =
      "history-command";


    commandElement.innerHTML =
      `
      <span class="terminal-prompt">
        marcus@portfolio:~$
      </span>

      <span></span>
      `;


    commandElement
      .querySelector(
        "span:last-child"
      )
      .textContent =
        command;


    terminalHistory
      .appendChild(
        commandElement
      );


    if (output) {

      const outputElement =
        document.createElement(
          "div"
        );

      outputElement.className =
        "history-output";


      if (isError) {

        outputElement
          .classList
          .add(
            "history-error"
          );

      }


      outputElement.textContent =
        output.trim();


      terminalHistory
        .appendChild(
          outputElement
        );

    }


    terminal.scrollIntoView({
      behavior: reducedMotion ? "auto" : "smooth",
      block: "nearest"
    });

  }


  /* -------------------------
     Handle command
  ------------------------- */

  function executeCommand(
    rawCommand
  ) {

    const command =
      rawCommand
        .trim()
        .toLowerCase();


    if (!command) {

      addHistory(
        ""
      );

      return;

    }


    if (
      command === "clear"
    ) {

      terminalHistory.innerHTML =
        "";

      return;
    }


    if (
      command === "projects"
    ) {

      addHistory(
        command,
        "Opening projects..."
      );


      setTimeout(
        function () {

          window.location.href =
            {{ "/projects/" | relative_url | jsonify }};

        },
        400
      );


      return;
    }


    if (
      Object.prototype.hasOwnProperty.call(commands, command)
    ) {

      addHistory(
        command,
        commands[command]
      );

      return;
    }


    addHistory(
      command,
      `Command not found: ${command}

Type "help" to see available commands.`,
      true
    );

  }


  /* -------------------------
     Input listener
  ------------------------- */

  terminalInput
    .addEventListener(
      "keydown",
      function (event) {

        if (
          event.key === "Enter"
        ) {

          const command =
            terminalInput.value;

          terminalInput.value =
            "";

          executeCommand(
            command
          );

        }

      }
    );


  /* Click terminal to focus */

  terminal
    .addEventListener(
      "click",
      function (event) {

        if (
          !event.target.closest("a, button, input") &&
          !window.getSelection().toString()
        ) {

          terminalInput.focus();

        }

      }
    );

});
</script>
