---
layout: single
title: "Resume"
permalink: /resume/
author_profile: false
classes: wide
description: "Marcus Toh — education, technical skills, and interests in software, AI, and robotics."
photo: /assets/images/IMG_7679.jpg
photo_alt: "Marcus Toh"
---

<div class="resume">
  <header class="resume-header">
    <div class="resume-header-content">
    <h2 class="resume-name">{{ site.author.name | escape }}</h2>
    <p class="resume-eyebrow">B.Eng Computer Science &amp; Design</p>
    <p class="resume-intro">Final-year undergraduate student at the Singapore University of Technology and Design</p>
    <ul class="resume-contact" aria-label="Contact and profiles">
      {% for link in site.author.links %}
      {% if link.url and link.url != "" %}
      <li><a href="{{ link.url | escape }}">{% if link.icon %}<i class="{{ link.icon | escape }}" aria-hidden="true"></i> {% endif %}{{ link.label | escape }}</a></li>
      {% endif %}
      {% endfor %}
    </ul>
    <button class="btn btn--primary resume-print" type="button" hidden>Print / Save as PDF</button>
    </div>
    <img class="resume-photo" src="{{ page.photo | relative_url }}" alt="{{ page.photo_alt | escape }}" width="150" height="180">
  </header>

  <section class="resume-section" aria-labelledby="resume-profile">
    <h2 id="resume-profile">Profile</h2>
    <p>I enjoy solving practical problems with technology and working with others to develop useful solutions. I bring perseverance, a willingness to learn, and experience across software, AI, and robotics.</p>
  </section>

  <section class="resume-section" aria-labelledby="resume-education">
    <h2 id="resume-education">Education</h2>
    <div class="resume-entry">
      <div class="resume-entry-heading">
        <h3>Singapore University of Technology and Design</h3>
        <p class="resume-dates"><time datetime="2023-09">Sep 2023</time> - Present</p>
      </div>
      <ul class="resume-details">
        <li>Bachelor of Engineering (Computer Science and Design)</li>
        <li>Minor in Artificial Intelligence</li>
        <li>Specialisation: Cybersecurity (Tentative)</li>
        <li>Expected Date of Graduation: <time datetime="2027-05">May 2027</time></li>
      </ul>
      <br>
      <div class="resume-entry-heading">
        <h3>Ngee Ann Polytechnic</h3>
        <p class="resume-dates"><time datetime="2021-04">Apr 2021</time> - Mar 2023</p>
      </div>
      <ul class="resume-details">
        <li>Diploma in Electronic &amp; Computer Engineering</li>
        <li>Specialisation: Robotics</li>
        <li>GPA: 3.51/4.0</li>
        <li>Named to the Director's List twice</li>
      </ul>
    </div>
  </section>

  <section class="resume-section" aria-labelledby="resume-experience">
    <h2 id="resume-experience">Professional Experience</h2>
    <div class="resume-entry">
      <div class="resume-entry-heading">
        <h3>Oneberry Technologies</h3>
        <p class="resume-dates"><time datetime="2025-09">Sep</time> – Dec 2025</p>
      </div>
      <p class="resume-role"><em>Robotics Engineer Intern</em></p>
      <ul class="resume-details">
        <li>Customised and trained open-source models, including Roboflow RF-DETR and DINOv2, for research into AI-assisted object detection and classification.</li>
        <li>Contributed to an Electron application serving as a user interface for robots. Customised an OpenAI chatbot and implemented Google Drive and Dropbox API integrations.</li>
      </ul>
    </div>
    <div class="resume-entry">
      <div class="resume-entry-heading">
        <h3>Accenture Southeast Asia</h3>
        <p class="resume-dates"><time datetime="2022-03">Mar</time> – Aug 2022</p>
      </div>
      <p class="resume-role"><em>Application Developer Intern</em></p>
      <ul class="resume-details">
        <li>Automated manual workflows using Power Automate and PowerShell to improve efficiency and save time.</li>
        <li>Developed activities in Pega CRMS to help monitor key server parameters.</li>
      </ul>
    </div>
  </section>


  <section class="resume-section" aria-labelledby="resume-projects">
    <h2 id="resume-projects">Projects</h2>
    <div class="resume-entry">
      <p>Explore my academic, personal, and internship projects.</p>
      <p><a href="{{ '/projects/' | relative_url }}">View Projects &rarr;</a></p>
    </div>
  </section>
  
  <section class="resume-section" aria-labelledby="resume-skills">
    <h2 id="resume-skills">Technical Skills</h2>
    <dl class="resume-skills">
      <div><dt>Programming</dt><dd>Python, Java, C, C++, C#</dd></div>
      <div><dt>Artificial Intelligence</dt><dd>PyTorch, OpenCV, OpenVINO</dd></div>
      <div><dt>Application Development</dt><dd>Flutter, Android (Java)</dd></div>
      <div><dt>Robotics</dt><dd>ROS, ROS 2, Computer Vision on Robots</dd></div>
      <div><dt>Hardware</dt><dd>Internet of Things, Arduino</dd></div>
      <div><dt>Data Analysis</dt><dd>Data Processing, Data Visualisation</dd></div>
    </dl>
  </section>

</div>

<style>
.resume { max-width: 900px; font-size: 0.9em; }
.resume-header { display: grid; grid-template-columns: minmax(0, 1fr) 150px; align-items: start; gap: 1.5rem; padding-bottom: 1.5rem; border-bottom: 3px solid #287b91; }
.resume-header-content { min-width: 0; }
.resume .resume-photo { width: 150px; height: 180px; margin: 0; object-fit: cover; border: 1px solid #d5d9dc; border-radius: 6px; }
.resume-contact i { margin-right: 0.2em; }
.resume-eyebrow { margin: 0 0 0.5rem; font-size: 0.75em; font-weight: 700; letter-spacing: 0.1em; text-transform: uppercase; }
.resume .resume-name { margin: 0; padding: 0; border: 0; font-size: clamp(2rem, 5vw, 3rem); line-height: 1.15; }
.resume-intro { max-width: 65ch; margin-top: 1rem; }
.resume-contact { display: flex; flex-wrap: wrap; gap: 0.75rem 2rem; padding: 0; list-style: none; }
.resume-contact li { margin: 0; }
.resume-print { margin-top: 0.5rem; }
.resume-print[hidden] { display: none; }
.resume-section { margin-top: 2rem; }
.resume-section > h2 { margin: 0 0 1rem; padding-bottom: 0.5rem; font-size: 1.2em; }
.resume-entry h3 { margin: 0 0 0.4rem; font-size: 1em; }
.resume-entry-heading { display: flex; justify-content: space-between; align-items: baseline; gap: 0.25rem 1.5rem; }
.resume-entry-heading h3 { margin: 0; line-height: 1.5; }
.resume .resume-role { margin: 0 0 0.4rem; line-height: 1.5; }
.resume .resume-dates { flex-shrink: 0; margin: 0; font-weight: 700; line-height: 1.5; white-space: nowrap; }
.resume .resume-details { margin: 0.15rem 0 0; padding-left: 1.6em; line-height: 1.5; }
.resume .resume-details li { margin-bottom: 0; }
.resume-entry + .resume-entry { margin-top: 1.5rem; }
.resume-meta { margin-bottom: 0.4rem; font-size: 0.9em; }
.resume-skills { display: grid; grid-template-columns: repeat(2, minmax(0, 1fr)); gap: 1.2rem 2rem; }
.resume-skills dt { margin: 0 0 0.3rem; font-weight: 700; }
.resume-skills dd { margin: 0; }
.resume a:focus-visible, .resume button:focus-visible { outline: 3px solid #287b91; outline-offset: 4px; }
@media (max-width: 600px) {
  .resume-header { grid-template-columns: minmax(0, 1fr) 90px; gap: 0.75rem; }
  .resume .resume-photo { width: 90px; height: 108px; }
  .resume-entry-heading { flex-direction: column; }
  .resume-skills { grid-template-columns: 1fr; }
}
@media print {
  @page { margin: 15mm; }
  body, #main, .page, .page__inner-wrap, .page__content { margin: 0 !important; padding: 0 !important; width: 100% !important; max-width: none !important; float: none !important; }
  body, .resume { background: #fff !important; color: #000 !important; font-size: 10pt; }
  .masthead, .sidebar, .page__footer, .page__meta, .page__share, .page__related, .pagination, .breadcrumbs, .search-content, .skip-links, .page__inner-wrap > header, .page__inner-wrap > footer, .resume-print { display: none !important; }
  .resume-header { grid-template-columns: minmax(0, 1fr) 100px; gap: 1rem; padding-bottom: 0.6rem; }
  .resume .resume-photo { width: 100px; height: 120px; }
  .resume .resume-name { font-size: 24pt; }
  .resume-section { margin-top: 1rem; }
  .resume-entry-heading { flex-direction: row; }
  .resume-section > h2, .resume-entry h3 { break-after: avoid; }
  .resume-entry, .resume-skills > div { break-inside: avoid; }
  .resume-skills { grid-template-columns: repeat(2, minmax(0, 1fr)); gap: 0.6rem 1.5rem; }
  .resume a { color: #000 !important; }
  .resume-contact { display: block; font-size: 8pt; }
  .resume-contact a::after { content: " — " attr(href); overflow-wrap: anywhere; }
}
</style>

<script>
document.querySelector(".resume-print").addEventListener("click", function () {
  window.print();
});
document.querySelector(".resume-print").hidden = false;
</script>
