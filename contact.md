---
layout: page
title: Contact detail
subtitle: ''
head-title: ""
css: "../css/custom.css"
---

Have a question, an exciting new idea or need to discuss matters? I'm always looking forward to friendly communication. You can find all the necessary details in order to make contact below.

##### Office:

- F-09 Telecommunication and Networking ([TeleCoN](https://www.giki.edu.pk/telecon)) Lab, 
  Faculty of Electrical Engineering, 
  [Ghulam Ishaq Khan (GIK) Institute of Engineering Sciences and Technology](https://www.giki.edu.pk/) 
  Topi-23640, Swabi, KPK, Pakistan.


##### Email:
[<img src="../img/email.png" height="40px">](mailto:arifullah@giki.edu.pk) [arifullah@giki.edu.pk](mailto:arifullah@giki.edu.pk)
[<img src="../img/gmail.png" height="40px">](mailto:arifullah@giki.edu.pk) [engrz.ciit@gmail.com](mailto:engrz.ciit@gmail.com)
  
##### linkedin Profile:
[<img src="../img/linkedin.png" height="40px">](https://www.linkedin.com/in/arifullah012/)

You can also send me a quick message using the form below:
{% macro errorList(errors) %}
    {% if errors %}
        <ul class="errors">
            {% for error in errors %}
                <li>{{ error }}</li>
            {% endfor %}
        </ul>
    {% endif %}
{% endmacro %}

{% from _self import errorList %}

<form method="post" action="" accept-charset="UTF-8">
    {{ csrfInput() }}
    <input type="hidden" name="action" value="contact-form/send">
    {{ redirectInput('contact/thanks') }}

    <h3><label for="from-name">Your Name</label></h3>
    <input id="from-name" type="text" name="fromName" value="{{ message.fromName ?? '' }}">
    {{ message is defined and message ? errorList(message.getErrors('fromName')) }}

    <h3><label for="from-email">Your Email</label></h3>
    <input id="from-email" type="email" name="fromEmail" value="{{ message.fromEmail ?? '' }}">
    {{ message is defined and message ? errorList(message.getErrors('fromEmail')) }}

    <h3><label for="subject">Subject</label></h3>
    <input id="subject" type="text" name="subject" value="{{ message.subject ?? '' }}">
    {{ message is defined and message ? errorList(message.getErrors('subject')) }}

    <h3><label for="message">Message</label></h3>
    <textarea rows="10" cols="40" id="message" name="message">{{ message.message ?? '' }}</textarea>
    {{ message is defined and message ? errorList(message.getErrors('message')) }}

    <input type="submit" value="Send">
</form>
