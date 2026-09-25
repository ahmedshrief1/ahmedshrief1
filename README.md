<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Ahmed Shrief | AI Automation Engineer &amp; n8n Automation Specialist</title>
<meta name="description" content="AI Automation Engineer specializing in n8n workflow automation, AI agents, multi-agent workflows, REST APIs, webhooks, and AI-powered business process automation.">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,500;0,600;1,400&family=Inter:wght@300;400;500;600&display=swap" rel="stylesheet">
<style>

:root{
  --bg:#050505;
  --bg-2:#0A0A0A;
  --gold:#D4AF37;
  --gold-soft:#E5C76B;
  --text:#F5F5F5;
  --text-2:#9A9A9A;
  --border:rgba(212,175,55,0.18);
  --serif:'Playfair Display', Georgia, serif;
  --sans:'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
  --ease:cubic-bezier(.22,1,.36,1);
}

*{margin:0;padding:0;box-sizing:border-box;}
html{scroll-behavior:smooth;}
body{
  background:var(--bg);
  color:var(--text);
  font-family:var(--sans);
  font-weight:300;
  line-height:1.6;
  overflow-x:hidden;
  -webkit-font-smoothing:antialiased;
}
::selection{background:var(--gold);color:#050505;}

img{max-width:100%;display:block;}
a{color:inherit;text-decoration:none;}
button{font-family:inherit;cursor:pointer;background:none;border:none;color:inherit;}

.wrap{max-width:1180px;margin:0 auto;padding:0 40px;}

@media (max-width:640px){
  .wrap{padding:0 24px;}
}

/* reveal */
.reveal{opacity:0;transform:translateY(28px);transition:opacity 1s var(--ease), transform 1s var(--ease);}
.reveal.in{opacity:1;transform:translateY(0);}
@media (prefers-reduced-motion:reduce){
  .reveal{opacity:1;transform:none;transition:none;}
  html{scroll-behavior:auto;}
}

.eyebrow{
  font-size:12px;
  letter-spacing:0.22em;
  text-transform:uppercase;
  color:var(--gold-soft);
  font-weight:500;
  display:flex;
  align-items:center;
  gap:12px;
}
.eyebrow::before{
  content:'';
  width:28px;height:1px;
  background:var(--gold);
  display:inline-block;
}

/* NAV */
header{
  position:fixed;top:0;left:0;right:0;
  z-index:100;
  padding:26px 0;
  transition:padding .5s var(--ease), background .5s var(--ease), border-color .5s var(--ease);
  border-bottom:1px solid transparent;
}
header.scrolled{
  padding:16px 0;
  background:rgba(5,5,5,0.82);
  backdrop-filter:blur(14px);
  -webkit-backdrop-filter:blur(14px);
  border-bottom:1px solid var(--border);
}
.nav-inner{
  display:flex;align-items:center;justify-content:space-between;
}
.brand{
  font-family:var(--serif);
  font-size:19px;
  letter-spacing:0.04em;
  font-style:italic;
}
.nav-links{
  display:flex;gap:38px;
  font-size:12px;
  letter-spacing:0.16em;
  text-transform:uppercase;
}
.nav-links a{
  position:relative;
  color:var(--text-2);
  transition:color .35s;
  padding:4px 0;
}
.nav-links a::after{
  content:'';
  position:absolute;left:0;bottom:0;
  width:0;height:1px;
  background:var(--gold);
  transition:width .4s var(--ease);
}
.nav-links a:hover,
.nav-links a.active{color:var(--text);}
.nav-links a:hover::after,
.nav-links a.active::after{width:100%;}

.nav-toggle{
  display:none;
  width:34px;height:34px;
  border:1px solid var(--border);
  border-radius:50%;
  align-items:center;justify-content:center;
  position:relative;
}
.nav-toggle span, .nav-toggle span::before, .nav-toggle span::after{
  content:'';
  position:absolute;
  width:12px;height:1px;
  background:var(--gold);
  transition:transform .3s;
}
.nav-toggle span::before{transform:translateY(-4px);}
.nav-toggle span::after{transform:translateY(4px);}

.mobile-panel{
  position:fixed;inset:0;
  background:rgba(5,5,5,0.98);
  z-index:99;
  display:flex;flex-direction:column;
  align-items:flex-start;
  justify-content:center;
  gap:26px;
  padding:0 40px;
  opacity:0;pointer-events:none;
  transition:opacity .4s var(--ease);
}
.mobile-panel.open{opacity:1;pointer-events:all;}
.mobile-panel a{
  font-family:var(--serif);
  font-size:32px;
  color:var(--text-2);
}
.mobile-panel a:hover{color:var(--gold);}

@media (max-width:880px){
  .nav-links{display:none;}
  .nav-toggle{display:flex;}
}

/* HERO */
.hero{
  min-height:100svh;
  display:flex;align-items:center;
  position:relative;
  padding-top:120px;padding-bottom:80px;
  background:
    radial-gradient(ellipse 60% 50% at 78% 30%, rgba(212,175,55,0.08), transparent 60%),
    var(--bg);
}
.hero-inner{
  display:grid;
  grid-template-columns:1.15fr 0.85fr;
  gap:40px;
  align-items:center;
  width:100%;
}
.hero-headline{
  font-family:var(--serif);
  font-size:clamp(52px, 8vw, 108px);
  line-height:0.98;
  font-weight:500;
  letter-spacing:-0.01em;
  margin:26px 0 28px;
}
.hero-desc{
  max-width:480px;
  color:var(--text-2);
  font-size:16px;
  line-height:1.75;
  margin-bottom:40px;
}
.cta-row{display:flex;gap:18px;flex-wrap:wrap;margin-bottom:56px;}
.btn{
  padding:16px 30px;
  font-size:12px;
  letter-spacing:0.14em;
  text-transform:uppercase;
  border-radius:2px;
  transition:transform .4s var(--ease), background .35s, color .35s, border-color .35s;
  display:inline-block;
}
.btn-primary{
  background:var(--gold);
  color:#0a0a0a;
  font-weight:500;
}
.btn-primary:hover{background:var(--gold-soft);}
.btn-outline{
  border:1px solid var(--border);
  color:var(--text);
}
.btn-outline:hover{border-color:var(--gold);color:var(--gold-soft);}

.hero-contact{
  display:flex;gap:34px;flex-wrap:wrap;
  font-size:13px;color:var(--text-2);
  border-top:1px solid var(--border);
  padding-top:24px;
}
.hero-contact a:hover{color:var(--gold-soft);}

/* hero visual: node lattice */
.hero-visual{position:relative;height:520px;}
.hero-visual svg{width:100%;height:100%;}
.node-dot{fill:var(--gold);}
.node-ring{fill:none;stroke:var(--border);stroke-width:1;}
.node-line{
  fill:none;stroke:rgba(212,175,55,0.35);stroke-width:1;
  stroke-dasharray:5 7;
  animation:dash 6s linear infinite;
}
@keyframes dash{to{stroke-dashoffset:-120;}}
.node-glow{fill:var(--gold);opacity:0.5;filter:blur(10px);}

@media (max-width:960px){
  .hero-inner{grid-template-columns:1fr;}
  .hero-visual{height:340px;order:-1;opacity:0.55;}
}

/* SECTION shared */
section{padding:150px 0;position:relative;}
@media (max-width:880px){section{padding:100px 0;}}
.section-head{max-width:640px;margin-bottom:76px;}
.section-head h2{
  font-family:var(--serif);
  font-size:clamp(34px,5vw,58px);
  line-height:1.08;
  font-weight:500;
  margin-top:18px;
}

/* ABOUT */
.about{background:var(--bg-2);border-top:1px solid var(--border);border-bottom:1px solid var(--border);}
.about-grid{
  display:grid;
  grid-template-columns:1.2fr 0.8fr;
  gap:90px;
  align-items:start;
}
.about-text p{color:var(--text-2);margin-bottom:22px;font-size:16px;max-width:52ch;}
.about-side{display:flex;flex-direction:column;gap:28px;}
.portrait-frame{
  border:1px solid var(--border);
  padding:10px;
  position:relative;
}
.portrait-frame img{filter:grayscale(0.15) contrast(1.05);}
.edu-panel{
  border:1px solid var(--border);
  padding:28px 30px;
  background:rgba(212,175,55,0.03);
}
.edu-panel .eyebrow{margin-bottom:14px;}
.edu-panel h3{font-family:var(--serif);font-size:20px;font-weight:500;margin-bottom:8px;}
.edu-panel p{color:var(--text-2);font-size:14px;}

@media (max-width:880px){
  .about-grid{grid-template-columns:1fr;gap:56px;}
}

/* AUTOMATION CARDS */
.cards-grid{
  display:grid;
  grid-template-columns:1fr 1fr;
  gap:1px;
  background:var(--border);
  border:1px solid var(--border);
}
.card{
  background:var(--bg);
  padding:52px 44px;
  transition:background .5s var(--ease);
}
.card:hover{background:var(--bg-2);}
.card-num{
  font-family:var(--serif);
  font-style:italic;
  color:var(--gold);
  font-size:15px;
  margin-bottom:26px;
  display:block;
}
.card h3{
  font-size:19px;
  letter-spacing:0.03em;
  font-weight:500;
  margin-bottom:16px;
}
.card p{color:var(--text-2);font-size:15px;max-width:38ch;}

@media (max-width:720px){
  .cards-grid{grid-template-columns:1fr;}
  .card{padding:40px 30px;}
}

/* N8N SECTION */
.n8n{background:var(--bg-2);border-top:1px solid var(--border);border-bottom:1px solid var(--border);}
.n8n-flow{
  display:flex;
  flex-direction:column;
  gap:0;
  margin-top:20px;
  max-width:420px;
}
.flow-node{
  border:1px solid var(--border);
  padding:20px 26px;
  font-size:13px;
  letter-spacing:0.12em;
  text-transform:uppercase;
  color:var(--text);
  position:relative;
  background:var(--bg);
}
.flow-node.active{border-color:var(--gold);color:var(--gold-soft);}
.flow-connector{
  height:44px;width:1px;
  background:var(--border);
  margin-left:26px;
  position:relative;
  overflow:hidden;
}
.flow-connector::after{
  content:'';
  position:absolute;top:-100%;left:0;
  width:100%;height:100%;
  background:linear-gradient(var(--gold), transparent);
  animation:flow 2.6s linear infinite;
}
@keyframes flow{
  0%{top:-100%;}
  100%{top:100%;}
}
.n8n-desc{color:var(--text-2);max-width:46ch;margin-top:24px;font-size:16px;}

.n8n-layout{
  display:grid;
  grid-template-columns:0.9fr 1.1fr;
  gap:80px;
  align-items:start;
}
@media (max-width:880px){
  .n8n-layout{grid-template-columns:1fr;gap:50px;}
}

/* FEATURED PROJECT */
.project-layout{
  display:grid;
  grid-template-columns:1fr 1fr;
  gap:90px;
  align-items:start;
}
.project-copy p{color:var(--text-2);margin-bottom:20px;font-size:15.5px;max-width:52ch;}
.meta-list{
  margin-top:44px;
  border-top:1px solid var(--border);
}
.meta-row{
  display:flex;justify-content:space-between;
  padding:18px 0;
  border-bottom:1px solid var(--border);
  font-size:13px;
}
.meta-row span:first-child{
  color:var(--text-2);
  letter-spacing:0.12em;
  text-transform:uppercase;
  font-size:11px;
}
.meta-row span:last-child{color:var(--gold-soft);font-family:var(--serif);font-size:16px;font-style:italic;}

.workflow-mock{
  border:1px solid var(--border);
  padding:44px 34px;
  background:var(--bg-2);
}
.wf-node{
  display:flex;align-items:center;gap:16px;
  padding:16px 0;
  border-bottom:1px dashed var(--border);
  font-size:13px;letter-spacing:0.08em;text-transform:uppercase;
  color:var(--text-2);
}
.wf-node:last-child{border-bottom:none;}
.wf-dot{
  width:7px;height:7px;border-radius:50%;
  background:var(--gold);
  flex-shrink:0;
}
.wf-node.hi{color:var(--text);}

@media (max-width:880px){
  .project-layout{grid-template-columns:1fr;gap:50px;}
}

/* SKILLS */
.skills-grid{
  display:grid;
  grid-template-columns:repeat(3,1fr);
  gap:60px;
}
.skill-col h3{
  font-family:var(--serif);
  font-style:italic;
  font-size:19px;
  color:var(--gold-soft);
  margin-bottom:22px;
  padding-bottom:16px;
  border-bottom:1px solid var(--border);
}
.skill-col ul{list-style:none;}
.skill-col li{
  color:var(--text-2);
  font-size:14.5px;
  padding:9px 0;
  transition:color .3s, padding-left .3s;
  cursor:default;
}
.skill-col li:hover{color:var(--text);padding-left:6px;}

@media (max-width:880px){
  .skills-grid{grid-template-columns:1fr 1fr;}
}
@media (max-width:560px){
  .skills-grid{grid-template-columns:1fr;}
}

/* TRAINING */
.training{background:var(--bg-2);border-top:1px solid var(--border);border-bottom:1px solid var(--border);}
.training-block{
  display:grid;
  grid-template-columns:0.7fr 1.3fr;
  gap:70px;
}
.training-org{
  font-family:var(--serif);
  font-size:24px;
  font-style:italic;
  color:var(--gold-soft);
  border-left:1px solid var(--gold);
  padding-left:24px;
}
.training-items{border-left:1px solid var(--border);}
.t-item{
  padding:0 0 32px 34px;
  position:relative;
}
.t-item::before{
  content:'';
  position:absolute;left:-4.5px;top:5px;
  width:8px;height:8px;border-radius:50%;
  background:var(--gold);
}
.t-item p{color:var(--text-2);font-size:15px;max-width:56ch;}

@media (max-width:760px){
  .training-block{grid-template-columns:1fr;gap:36px;}
}

/* PHILOSOPHY */
.philosophy{
  text-align:left;
  padding:190px 0;
}
.philosophy .wrap{max-width:900px;}
.phil-heading{
  font-family:var(--serif);
  font-weight:500;
  font-size:clamp(36px,6vw,64px);
  line-height:1.12;
}
.phil-heading .line{
  display:block;
  overflow:hidden;
}
.phil-heading .line span{
  display:block;
  transform:translateY(110%);
  transition:transform 1s var(--ease);
}
.phil-heading.in .line span{transform:translateY(0);}
.phil-heading .line:nth-child(2) span{transition-delay:.08s;}
.phil-heading .line:nth-child(3) span{transition-delay:.16s;}
.phil-heading .line:nth-child(4) span{transition-delay:.24s;}
.phil-sub{
  color:var(--text-2);
  font-size:16px;
  max-width:50ch;
  margin-top:34px;
}

/* CONTACT */
.contact{background:var(--bg-2);border-top:1px solid var(--border);}
.contact-grid{
  display:grid;grid-template-columns:1.2fr 0.8fr;
  gap:70px;align-items:end;
}
.contact-heading{
  font-family:var(--serif);
  font-size:clamp(44px,8vw,92px);
  line-height:0.98;
  font-weight:500;
}
.contact-desc{color:var(--text-2);margin-top:24px;max-width:44ch;font-size:16px;}
.contact-info{border-top:1px solid var(--border);padding-top:28px;}
.contact-info .name{font-family:var(--serif);font-style:italic;font-size:20px;margin-bottom:16px;}
.contact-info div{color:var(--text-2);font-size:14.5px;margin-bottom:8px;}
.contact-info a:hover{color:var(--gold-soft);}
.contact-btns{display:flex;gap:16px;margin-top:30px;flex-wrap:wrap;}

@media (max-width:880px){
  .contact-grid{grid-template-columns:1fr;gap:46px;align-items:start;}
}

/* FOOTER */
footer{padding:50px 0;}
.footer-inner{
  display:flex;justify-content:space-between;align-items:center;
  flex-wrap:wrap;gap:14px;
  border-top:1px solid var(--border);
  padding-top:34px;
}
.footer-brand{font-family:var(--serif);font-style:italic;font-size:16px;}
.footer-role{font-size:11px;letter-spacing:0.16em;text-transform:uppercase;color:var(--text-2);}
.footer-copy{font-size:12.5px;color:var(--text-2);}

</style>
</head>
<body>

<header id="siteHeader">
  <div class="wrap nav-inner">
    <div class="brand">Ahmed Shrief</div>
    <nav class="nav-links" id="navLinks">
      <a href="#home" class="nav-a" data-target="home">Home</a>
      <a href="#about" class="nav-a" data-target="about">About</a>
      <a href="#automation" class="nav-a" data-target="automation">Automation</a>
      <a href="#project" class="nav-a" data-target="project">Project</a>
      <a href="#skills" class="nav-a" data-target="skills">Skills</a>
      <a href="#training" class="nav-a" data-target="training">Training</a>
      <a href="#contact" class="nav-a" data-target="contact">Contact</a>
    </nav>
    <button class="nav-toggle" id="navToggle" aria-label="Open menu"><span></span></button>
  </div>
</header>

<div class="mobile-panel" id="mobilePanel">
  <a href="#home" class="mob-a">Home</a>
  <a href="#about" class="mob-a">About</a>
  <a href="#automation" class="mob-a">Automation</a>
  <a href="#project" class="mob-a">Project</a>
  <a href="#skills" class="mob-a">Skills</a>
  <a href="#training" class="mob-a">Training</a>
  <a href="#contact" class="mob-a">Contact</a>
</div>

<section class="hero" id="home">
  <div class="wrap hero-inner">
    <div>
      <div class="eyebrow">AI Automation Engineer</div>
      <h1 class="hero-headline">Building<br>AI&#8209;Powered<br>Automation</h1>
      <p class="hero-desc">Designing and building AI-powered workflow automation systems with n8n, AI agents, REST APIs, webhooks, and workflow orchestration.</p>
      <div class="cta-row">
        <a href="#project" class="btn btn-primary" id="magBtn">View My Project</a>
        <a href="#contact" class="btn btn-outline">Let's Connect</a>
      </div>
      <div class="hero-contact">
        <a href="tel:01092353370">01092353370</a>
        <a href="mailto:ahmedshrief796@gmail.com">ahmedshrief796@gmail.com</a>
        <a href="https://www.linkedin.com/in/ahmad-shrief" target="_blank" rel="noopener">LinkedIn</a>
      </div>
    </div>
    <div class="hero-visual" aria-hidden="true">
      <svg viewBox="0 0 400 520" xmlns="http://www.w3.org/2000/svg">
        <circle class="node-ring" cx="200" cy="120" r="90"/>
        <circle class="node-ring" cx="200" cy="120" r="150"/>
        <path class="node-line" d="M200,30 L200,260"/>
        <path class="node-line" d="M50,120 L350,120"/>
        <path class="node-line" d="M90,260 L310,380"/>
        <path class="node-line" d="M310,260 L90,380"/>
        <circle class="node-glow" cx="200" cy="120" r="10"/>
        <circle class="node-dot" cx="200" cy="120" r="4.5"/>
        <circle class="node-dot" cx="200" cy="30" r="3.5"/>
        <circle class="node-dot" cx="200" cy="260" r="3.5"/>
        <circle class="node-dot" cx="50" cy="120" r="3.5"/>
        <circle class="node-dot" cx="350" cy="120" r="3.5"/>
        <circle class="node-dot" cx="90" cy="260" r="3.5"/>
        <circle class="node-dot" cx="310" cy="260" r="3.5"/>
        <circle class="node-dot" cx="90" cy="380" r="3.5"/>
        <circle class="node-dot" cx="310" cy="380" r="3.5"/>
        <circle class="node-ring" cx="200" cy="440" r="50"/>
        <circle class="node-dot" cx="200" cy="440" r="4"/>
      </svg>
    </div>
  </div>
</section>

<section class="about" id="about">
  <div class="wrap about-grid">
    <div class="about-text reveal">
      <div class="eyebrow">About</div>
      <h2 class="section-head" style="margin-bottom:34px;">Automation<br>with purpose.</h2>
      <p>Computer Science undergraduate at Fayoum University specializing in AI Automation Engineering, focused on designing and building AI-powered workflow automation systems with n8n.</p>
      <p>Skilled in developing multi-agent AI workflows that orchestrate business processes end-to-end, integrating REST APIs, webhooks, and third-party services to reduce manual work and streamline operations.</p>
      <p>Trained through the Digital Egypt Pioneers Initiative (DEPI) in automation engineering practices, with a practical foundation in Python and machine learning fundamentals applied to workflow logic and data processing.</p>
    </div>
    <div class="about-side reveal">
      <div class="portrait-frame">
        <img src="data:image/jpeg;base64,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" alt="Portrait of Ahmed Shrief Abd El-Ghaffar">
      </div>
      <div class="edu-panel">
        <div class="eyebrow">Education</div>
        <h3>Bachelor of Computer Science</h3>
        <p>Faculty of Computers and Information, Fayoum University<br>2024 &ndash; 2028 &middot; Egypt</p>
      </div>
    </div>
  </div>
</section>

<section id="automation">
  <div class="wrap">
    <div class="section-head reveal">
      <div class="eyebrow">What I Build</div>
      <h2>AI automation<br>systems.</h2>
    </div>
    <div class="cards-grid reveal">
      <div class="card">
        <span class="card-num">01</span>
        <h3>AI Workflow Automation</h3>
        <p>AI-powered workflows designed to automate repetitive business processes and connect different systems.</p>
      </div>
      <div class="card">
        <span class="card-num">02</span>
        <h3>AI Agents</h3>
        <p>AI agents integrated into workflows to handle specialized tasks and decision-making stages.</p>
      </div>
      <div class="card">
        <span class="card-num">03</span>
        <h3>Multi-Agent Workflows</h3>
        <p>Multiple AI agents connected through structured workflow orchestration, with each agent assigned a distinct role.</p>
      </div>
      <div class="card">
        <span class="card-num">04</span>
        <h3>API &amp; System Integration</h3>
        <p>REST APIs, HTTP Requests, Webhooks, JSON, authentication, and third-party integrations.</p>
      </div>
    </div>
  </div>
</section>

<section class="n8n" id="n8n-visual">
  <div class="wrap n8n-layout">
    <div class="reveal">
      <div class="eyebrow">n8n</div>
      <h2 class="section-head" style="margin-bottom:0;">The engine<br>behind the workflow.</h2>
      <p class="n8n-desc">n8n workflow development and automation with triggers, nodes, HTTP Request, Webhooks, Conditional Logic, API Integrations, and workflow orchestration.</p>
    </div>
    <div class="n8n-flow reveal">
      <div class="flow-node active">Trigger</div>
      <div class="flow-connector"></div>
      <div class="flow-node">Data</div>
      <div class="flow-connector"></div>
      <div class="flow-node active">AI Agent</div>
      <div class="flow-connector"></div>
      <div class="flow-node">Conditional Logic</div>
      <div class="flow-connector"></div>
      <div class="flow-node">API</div>
      <div class="flow-connector"></div>
      <div class="flow-node active">Output</div>
    </div>
  </div>
</section>

<section id="project">
  <div class="wrap">
    <div class="section-head reveal">
      <div class="eyebrow">Featured Project</div>
      <h2>n8n HR multi-agent<br>workflow.</h2>
    </div>
    <div class="project-layout">
      <div class="project-copy reveal">
        <p>Designed and built an automated HR workflow using n8n as the core workflow orchestration platform, structuring the process into clear, sequential automation steps.</p>
        <p>Architected a multi-agent workflow by connecting multiple AI agents within n8n, assigning each agent a distinct role to collaboratively handle different stages of the HR process.</p>
        <p>Automated HR-related tasks by defining triggers, nodes, and conditional logic to route information and decisions through the workflow without manual intervention.</p>
        <p>Integrated external services and APIs into the workflow using HTTP Request nodes and webhooks to enable data exchange between n8n and third-party systems.</p>
        <p>Tested and refined workflow execution paths to improve reliability, handling edge cases and validating outputs at each stage of the automation.</p>
        <p>Applied AI automation principles to translate a manual HR process into a practical, AI-powered automation system.</p>

        <div class="meta-list">
          <div class="meta-row"><span>Role</span><span>AI Automation Engineer</span></div>
          <div class="meta-row"><span>Core Technology</span><span>n8n</span></div>
          <div class="meta-row"><span>Focus</span><span>Multi-Agent AI Workflow</span></div>
          <div class="meta-row"><span>Integration</span><span>REST APIs / Webhooks</span></div>
        </div>
      </div>

      <div class="workflow-mock reveal">
        <div class="wf-node hi"><span class="wf-dot"></span>Trigger</div>
        <div class="wf-node hi"><span class="wf-dot"></span>AI Agent</div>
        <div class="wf-node"><span class="wf-dot"></span>HR Processing</div>
        <div class="wf-node"><span class="wf-dot"></span>Conditional Logic</div>
        <div class="wf-node"><span class="wf-dot"></span>API</div>
        <div class="wf-node hi"><span class="wf-dot"></span>Output</div>
      </div>
    </div>
  </div>
</section>

<section id="skills">
  <div class="wrap">
    <div class="section-head reveal">
      <div class="eyebrow">Technical Stack</div>
      <h2>Tools and<br>capabilities.</h2>
    </div>
    <div class="skills-grid reveal">
      <div class="skill-col">
        <h3>AI Automation</h3>
        <ul>
          <li>AI Workflow Automation</li>
          <li>Business Process Automation</li>
          <li>AI Agents</li>
          <li>Multi-Agent Workflows</li>
          <li>Workflow Orchestration</li>
          <li>Automation Logic</li>
        </ul>
      </div>
      <div class="skill-col">
        <h3>n8n</h3>
        <ul>
          <li>n8n Workflow Development</li>
          <li>Workflow Automation</li>
          <li>Triggers</li>
          <li>Nodes</li>
          <li>HTTP Request</li>
          <li>Webhooks</li>
          <li>Conditional Logic</li>
          <li>API Integrations</li>
        </ul>
      </div>
      <div class="skill-col">
        <h3>APIs &amp; Integrations</h3>
        <ul>
          <li>REST APIs</li>
          <li>GET Requests</li>
          <li>POST Requests</li>
          <li>JSON</li>
          <li>Webhooks</li>
          <li>API Authentication</li>
          <li>Third-Party Integrations</li>
        </ul>
      </div>
      <div class="skill-col">
        <h3>AI &amp; Programming</h3>
        <ul>
          <li>Python</li>
          <li>AI Fundamentals</li>
          <li>Machine Learning Fundamentals</li>
          <li>Data Processing</li>
          <li>AI Model Integration</li>
          <li>LLM Integration</li>
        </ul>
      </div>
      <div class="skill-col">
        <h3>Technical Tools</h3>
        <ul>
          <li>n8n</li>
          <li>Python</li>
          <li>Git</li>
          <li>GitHub</li>
          <li>FastAPI</li>
          <li>REST APIs</li>
          <li>JSON</li>
        </ul>
      </div>
    </div>
  </div>
</section>

<section class="training" id="training">
  <div class="wrap">
    <div class="section-head reveal">
      <div class="eyebrow">Training</div>
      <h2>Digital Egypt<br>Pioneers Initiative.</h2>
    </div>
    <div class="training-block reveal">
      <div class="training-org">Digital Egypt Pioneers Initiative (DEPI)</div>
      <div class="training-items">
        <div class="t-item"><p>Completed hands-on training in AI Automation, covering n8n workflow automation, AI agents, and automation engineering practices.</p></div>
        <div class="t-item"><p>Practiced building and integrating REST APIs and webhooks within automated workflows as part of applied automation exercises.</p></div>
        <div class="t-item"><p>Developed workflow orchestration and automation logic skills through structured, project-based learning.</p></div>
      </div>
    </div>
  </div>
</section>

<section class="philosophy">
  <div class="wrap">
    <h2 class="phil-heading" id="philHeading">
      <span class="line"><span>From manual process</span></span>
      <span class="line"><span>to intelligent</span></span>
      <span class="line"><span>workflow.</span></span>
    </h2>
    <p class="phil-sub reveal">Building reliable, scalable AI automation solutions grounded in API integration and workflow orchestration design.</p>
  </div>
</section>

<section class="contact" id="contact">
  <div class="wrap contact-grid">
    <div class="reveal">
      <h2 class="contact-heading">Let's<br>automate.</h2>
      <p class="contact-desc">Have an automation idea or want to connect?</p>
    </div>
    <div class="contact-info reveal">
      <div class="name">Ahmed Shrief Abd El-Ghaffar</div>
      <div><a href="tel:01092353370">01092353370</a></div>
      <div><a href="mailto:ahmedshrief796@gmail.com">ahmedshrief796@gmail.com</a></div>
      <div><a href="https://www.linkedin.com/in/ahmad-shrief" target="_blank" rel="noopener">linkedin.com/in/ahmad-shrief</a></div>
      <div class="contact-btns">
        <a href="mailto:ahmedshrief796@gmail.com" class="btn btn-primary">Email Me</a>
        <a href="https://www.linkedin.com/in/ahmad-shrief" target="_blank" rel="noopener" class="btn btn-outline">LinkedIn</a>
      </div>
    </div>
  </div>
</section>

<footer>
  <div class="wrap footer-inner">
    <div>
      <div class="footer-brand">Ahmed Shrief</div>
      <div class="footer-role">AI Automation Engineer</div>
    </div>
    <div class="footer-copy">&copy; 2026 Ahmed Shrief. All rights reserved.</div>
  </div>
</footer>

<script>
// Header scroll state
const header = document.getElementById('siteHeader');
window.addEventListener('scroll', () => {
  header.classList.toggle('scrolled', window.scrollY > 40);
}, {passive:true});

// Mobile menu
const navToggle = document.getElementById('navToggle');
const mobilePanel = document.getElementById('mobilePanel');
navToggle.addEventListener('click', () => mobilePanel.classList.toggle('open'));
document.querySelectorAll('.mob-a').forEach(a => {
  a.addEventListener('click', () => mobilePanel.classList.remove('open'));
});

// Reveal on scroll
const revealObserver = new IntersectionObserver((entries) => {
  entries.forEach(entry => {
    if(entry.isIntersecting){
      entry.target.classList.add('in');
      revealObserver.unobserve(entry.target);
    }
  });
}, {threshold:0.15});
document.querySelectorAll('.reveal').forEach(el => revealObserver.observe(el));

// Philosophy text reveal
const philHeading = document.getElementById('philHeading');
const philObserver = new IntersectionObserver((entries) => {
  entries.forEach(entry => {
    if(entry.isIntersecting){
      philHeading.classList.add('in');
      philObserver.unobserve(philHeading);
    }
  });
}, {threshold:0.4});
philObserver.observe(philHeading);

// Nav active-section detection
const sections = ['home','about','automation','project','skills','training','contact'];
const navAs = document.querySelectorAll('.nav-a');
const sectionObserver = new IntersectionObserver((entries) => {
  entries.forEach(entry => {
    if(entry.isIntersecting){
      navAs.forEach(a => a.classList.toggle('active', a.dataset.target === entry.target.id));
    }
  });
}, {threshold:0.5, rootMargin:'-30% 0px -55% 0px'});
sections.forEach(id => {
  const el = document.getElementById(id);
  if(el) sectionObserver.observe(el);
});

// Subtle magnetic CTA
const magBtn = document.getElementById('magBtn');
magBtn.addEventListener('mousemove', (e) => {
  const rect = magBtn.getBoundingClientRect();
  const x = e.clientX - rect.left - rect.width/2;
  const y = e.clientY - rect.top - rect.height/2;
  magBtn.style.transform = `translate(${x*0.18}px, ${y*0.35}px)`;
});
magBtn.addEventListener('mouseleave', () => {
  magBtn.style.transform = 'translate(0,0)';
});
</script>
</body>
</html>
