---
layout: default
title: About
redirect_from:
  - /about/
---

<div class="intro">
  <img class="intro-photo" src="/assets/pranav.jpg" alt="Pranav Ram">
  <div class="intro-text">
    <p class="intro-name">Hi, I'm Pranav</p>
    <p class="intro-role">A junior studying CS @ CMU</p>
    <p class="intro-label">Previous internships</p>
    <ul class="internships">
      <li><img src="/assets/logos/salesforce.svg" alt="Salesforce"></li>
      <li><img class="paraform" src="/assets/logos/paraform.svg" alt="Paraform"></li>
    </ul>
  </div>
</div>

<p class="intro-blurb">Interested in ML, Robotics, Math, Statistics, and positively impacting the world.</p>

<style>
.intro {
  display: grid;
  grid-template-columns: 200px 1fr;
  gap: 2rem;
  align-items: center;
  margin-top: 0.5rem;
}
.intro-photo {
  width: 200px;
  height: 240px;
  object-fit: cover;
  object-position: center 18%;
  border-radius: 6px;
  display: block;
}
.intro-name {
  font-size: 2.15rem;
  font-weight: 650;
  line-height: 1.1;
  letter-spacing: -0.03em;
  margin: 0 0 0.4rem;
}
.intro-role {
  font-size: 1.15rem;
  color: #555;
  margin: 0 0 1.35rem;
}
.intro-label {
  margin: 0 0 0.7rem;
  font-size: 0.75rem;
  letter-spacing: 0.06em;
  text-transform: uppercase;
  color: #888;
}
.internships {
  list-style: none;
  display: flex;
  align-items: center;
  gap: 1.35rem;
  margin: 0;
  padding: 0;
  flex-wrap: wrap;
}
.internships li {
  display: flex;
  align-items: center;
  margin: 0;
  height: 46px;
}
.internships img {
  display: block;
  height: 46px;
  width: auto;
}
.internships img.paraform {
  height: 22px;
}
.intro-blurb {
  max-width: 42rem;
  margin: 1.75rem 0 0;
  font-size: 1.05rem;
  line-height: 1.65;
  color: #333;
}
@media (max-width: 600px) {
  .intro {
    grid-template-columns: 1fr;
    justify-items: start;
  }
  .intro-photo {
    width: 160px;
    height: 192px;
  }
}
</style>
