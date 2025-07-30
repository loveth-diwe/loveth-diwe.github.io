---
layout: default
title: Home
---

<style>
/* Force side-by-side on desktop */
.hero-section{
  display:flex;
  flex-wrap:nowrap;          /* keep in one row on wide screens */
  gap:2rem;
  align-items:flex-start;
}
.left-side,.right-side{
  flex:1 1 50%;
  min-width:0;               /* prevents overflow issues */
}
.screen-container{
  position:relative;
  width:100%;
  max-width:700px;
}
.screen-container img{
  width:100%;
  height:auto;
  display:block;
  border-radius:12px;
}
.tagline{
  position:absolute;
  top:12px; left:12px;
  background:rgba(0,0,0,.75);
  color:#fff; padding:.45rem .8rem;
  border-radius:8px; font-weight:600;
}
.right-side{
  display:flex;
  flex-direction:column;     /* headshot above intro */
  align-items:flex-start;    /* keep to the left */
}
.headshot{
  width:120px; height:120px;
  border-radius:50%;
  object-fit:cover;
  margin-bottom:1rem;
  box-shadow:0 4px 12px rgba(0,0,0,.18);
}

/* On small screens, allow stacking */
@media (max-width: 800px){
  .hero-section{flex-wrap:wrap}
  .left-side,.right-side{flex:1 1 100%}
}
</style>

<!-- HERO SECTION -->
<div class="hero-section">
  <div class="left-side">
    <div class="screen-container">
      <img src="{{ '/assets/img/computer.jpg' | relative_url }}" alt="Computer Screen">
    </div>
  </div>

  <div class="right-side">
    <img class="headshot" src="{{ '/assets/img/me.jpg' | relative_url }}" alt="Loveth headshot">
    <h1>👋 Hi! I'm Loveth</h1>
    <p>
      An Enterprise Application Support Engineer with years of experience in implementations,
      integrations, and problem resolution while maintaining optimized performance.
    </p>
    <p>
      I have hands‑on experience in information security and system control, and I work well as part of a team of
      skilled engineers and operations management to improve organizational objectives and goals.
    </p>
    <p>Explore my:</p>
    <ul>
      <li><a href="{{ '/cv' | relative_url }}">CV</a></li>
      <li><a href="{{ '/projects' | relative_url }}">Projects</a></li>
      <li><a href="{{ '/trainings' | relative_url }}">Trainings</a></li>
    </ul>
  </div>
</div>
