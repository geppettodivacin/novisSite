---
layout: page
title: "contact"
footer: true
sidebar: false
---

<div class="grid">
  <div id="contact-div" class="col-2-3 grid">
    <form name="contactUsForm" action="confirm_contact" onsubmit="return validateForm();" method="post">
      <label for="name" class="col-1-2">Name</label>
      <label for="email" class="col-1-2">Email Address</label>
      <input type="text" name="name" value="Name" onclick="this.value='';" onfocus="this.select()" onblur="this.value=!this.value?'Name':this.value;" class="col-1-2" />
      <input type="text" name="email" value="Email" onclick="this.value='';" onfocus="this.select()" onblur="this.value=!this.value?'Email':this.value;" class="col-1-2" />
      <label for="social" class="col-1-2">How did you hear about us?</label>
      <label for="reason" class="col-1-2">Reason for Inquiry</label>
      <input type="text" name="social" value="Facebook, Twitter, Google, etc." onclick="this.value='';" onfocus="this.select()" onblur="this.value=!this.value?'Facebook, Twitter, Google, etc.':this.value;" class="col-1-2" />
      <input type="text" name="reason" value="Want to auditon/book/etc." onclick="this.value='';" onfocus="this.select()" onblur="this.value=!this.value?'Want to auditon/book/etc.':this.value;" class="col-1-2" />
      <label for="question" class="col-1-1">Message Area</label>
      <textarea name="question" onclick="this.value='';" onfocus="this.select()" onblur="this.value=!this.value?'Questions?':this.value;" class="col-1-1">Questions?</textarea>
      <p class="col-1-1"><button type="submit">Submit</button><button type="reset">Reset</button></p>
    </form>
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
