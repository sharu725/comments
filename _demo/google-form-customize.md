---
title: Google Custom Form
description: This is a demo of Customized Google Form.
article: /google-form-customize/
layout: demo
---


Here is a working form that you can check. I have restricted the entries to 18 characters so as to avoid long spams.

<style>
input {
    padding: 5px 10px;
    margin-bottom: 10px;
}
</style>

<script type="text/javascript">var submitted=false;</script>
<iframe name="hidden_iframe" id="hidden_iframe" style="display:none;"     
onload="if(submitted) {window.location='{{site.url}}{{page.url}}';}"></iframe>
<form action="https://docs.google.com/forms/d/e/1FAIpQLSdqGYth5-G2cP8SILJwjOcJ38vit-Rv8E9SXmtnJUu4ifMcGw/formResponse" method="post" target="hidden_iframe" 
onsubmit="submitted=true;">
      <label>Name</label>
      <input name="entry.742532386" type="text" maxlength="18" placeholder=" John Doe" />
      <br>
      <label>Email</label>
      <input name="entry.1558941179" type="email" required maxlength="18" placeholder=" john@email.com"/>
      <br>
      <input type="submit" value="Send" />

</form>

You can check the entries [here](https://docs.google.com/spreadsheets/d/1_vt8il8LpxEi8_DmX0yxxRambpw700cdMC2yMIGWqbk/edit?usp=sharing){: target="_blank"}.