---
layout: page
title_nav: Contact
title: Contact Us
permalink: /contact/
weight: 5
enabled: true
---

<div class="table-responsive">
  <table class="table">
    <tr>
      <td><strong>Phone:</strong></td>
      <td>{{ site.contact_number }}</td>
    </tr>
    <tr>
      <td><strong>Email:</strong></td>
      <td><a href="mailto:{{ site.email }}?subject=[MFC Bricklaying Website Enquiry]">{{ site.email }}</a></td>
    </tr>
    <tr>
      <td><strong>Facebook:</strong></td>
      <td><a href="https://facebook.com/{{ site.facebook_username }}">https://facebook.com/{{ site.facebook_username }}</a></td>
    </tr>
  </table>
</div>

<p>
  Feel free to contact us to request a free quotation or even if you would just like to ask a question. All calls will be happily taken.
</p><br />

<h4>Request a Quote</h4>
<p>Feel free to request a quote and we will get back to you as soon as possible.</p><br />

<form action="//formspree.io/{{ site.email }}" method="POST">
  <div class="form-group">
    <label for="email">Email:</label>
    <div class="input-group">
      <span class="input-group-addon" id="basic-addon1">@</span>
      <input type="email" class="form-control" name="_replyto">
    </div>
  </div>
  <div class="form-group">
    <label for="email">Job Description:</label>
    <textarea name="body" class="form-control" rows="8"></textarea>
  </div>

  <input type="submit" class="btn btn-success" value="Submit Request">
</form>
