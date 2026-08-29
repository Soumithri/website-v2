---
layout: layouts/base.njk
title: "Contact"
---

<section class="page-intro">
  <p class="section-kicker">Start a conversation</p>
  <h1 class="page-heading">Have a data problem worth solving?</h1>
  <p class="page-lede">Tell me what is stuck, what is changing, or what you want to make possible.</p>
</section>

<section id="contact" class="contact-form">
  <form action="https://formspree.io/f/your-form-id" method="POST">
    <div class="form-row">
      <div class="form-field">
        <label for="name">Name</label>
        <input id="name" name="name" required />
      </div>
      <div class="form-field">
        <label for="email">Email</label>
        <input id="email" name="email" type="email" required />
      </div>
    </div>
    <div class="form-field">
      <label for="message">What are you working on?</label>
      <textarea id="message" name="message" rows="7" required></textarea>
    </div>
    <button type="submit" class="button">Send inquiry</button>
  </form>
</section>
