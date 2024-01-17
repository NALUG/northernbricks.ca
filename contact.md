---
layout: page
title: Contact Us
permalink: /contact/
background: '/assets/minifigs.png'
---
  <script src="https://www.google.com/recaptcha/api.js?render=6Lfb8VMpAAAAAJQMQOlUkwdW7X2hjE5GHnQHDu7O"></script>
  <script>
    grecaptcha.ready(function () {
      grecaptcha
        .execute('6Lfb8VMpAAAAAJQMQOlUkwdW7X2hjE5GHnQHDu7O', {
          action: 'submit',
        })
        .then(function (token) {
          console.info('got token: ' + token);
          document.getElementById('g-recaptcha-response').value = token;
        });
    });
  </script>

<style>
    .form-row{
        padding-bottom:5px;
    }    
</style>
<!-- modify this form HTML and place wherever you want your form -->
<form
  action="https://formspree.io/f/xkndgyzp"
  method="POST"
>
    <input type="hidden" id="g-recaptcha-response" name="g-recaptcha-response">

<div class="form-row">
    <div class="col">
        <input type="text" class="form-control" name="Name" placeholder="Name">
    </div>
    <div class="col">
        <input type="text" class="form-control" name="Email" placeholder="Email">
    </div>
</div>

<div class="form-row">
    <div class="col">
        <input type="text" class="form-control" name="Subject" placeholder="Subject">
    </div>
</div>

<div class="form-row">
    <div class="col">
        <textarea class="form-control" name="Message" placeholder="Message" rows="4"></textarea>
    </div>
</div>
<div class="form-row">
    <div class="col">
        <button class="btn btn-primary" type="submit">Send</button>
    </div>
 </div>
</form>