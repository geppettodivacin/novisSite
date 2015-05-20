---
layout: page
title: "contact"
footer: true
sidebar: false
---

<div class="grid">
  <div class="col-2-3">
    {% google_form 1OYdFt2ZvcGzNvsxqTN8Mg_Xs4U129HaJpGIZeL4QC7g Thank you for contacting us. We will return your email as soon as possible. %}
  </div>

  <aside id="more-contact" class="side col-1-3">
    <h3>Additional Contact</h3>
    <ul>
      <li><h4>President:</h4>{{ site.contact.president.name }} - <a href="mailto:{{ site.contact.president.email }}">{{ site.contact.president.email }}</a></li>
      <li><h4>Director:</h4>{{ site.contact.director.name }} - <a href="mailto:{{ site.contact.director.email }}">{{ site.contact.director.email }}</a></li>
      <li><h4>Social Chair:</h4>{{ site.contact.social.name }} - <a href="mailto:{{ site.contact.social.email }}">{{ site.contact.social.email }}</a></li>
      <li><h4>Faculty Advisor:</h4>{{ site.contact.advisor.name }} - <a href="mailto:{{ site.contact.advisor.email }}">{{ site.contact.advisor.email }}</a></li>
    </ul>
  </aside>
</div>
