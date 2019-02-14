---
layout: video
title: STORE
sidebar_link: false
description: store.
author: Caleb Brenden
---
<h1 class="page-title" style="padding-top: 1rem;">STICKERS</h1>


<!-- PAYPAL BUTTON -->
<form target="paypal" action="https://www.paypal.com/cgi-bin/webscr" method="post">
<input type="hidden" name="cmd" value="_s-xclick">
<input type="hidden" name="hosted_button_id" value="UQA4V6R4QVEW6">
<table>
<tr><td><input type="hidden" name="on0" value="Stickers">Stickers</td></tr><tr><td><select name="os0">
	<option value="NM National Parks">NM National Parks $9.99 USD</option>
	<option value="Albuquerque, NM">Albuquerque, NM $3.00 USD</option>
	<option value="Shiprock, NM (Daytime)">Shiprock, NM (Daytime) $3.00 USD</option>
	<option value="Shiprock, NM (Nighttime)">Shiprock, NM (Nighttime) $3.00 USD</option>
</select> </td></tr>
</table>
<input type="hidden" name="currency_code" value="USD">
<input type="image" src="https://www.paypalobjects.com/en_US/i/btn/btn_cart_LG.gif" border="0" name="submit" alt="PayPal - The safer, easier way to pay online!">
</form>
<p>All of my designs are printed on durable vinyl stickers, which means they are UV protected, waterproof, and the designs don’t rub off!</p>
<h2>"ABQ"</h2>
<img src="{{ site.baseurl }}/images/design/abq-sticker.jpg" alt="abq sticker">
<p>Printed on waterproof, fade resistant vinyl, this 2.33"x3" sticker is great for slapping on your water bottle, laptop, or whatever the heck else you want!</p>
<h2>New Mexico National Parks & Monuments Sticker Sheet</h2>
<img src="{{ site.baseurl }}/images/design/sticker-sheet.jpg" alt="sticker sheet">
<p>Printed by my beautiful friends over at Sticker Ninja, this sticker sheet is 8"x10", and consists of 13 individual stickers.</p>
<h2>Santa Fe, NM - Daytime</h2>
  <img src="{{ site.baseurl }}/images/design/santa-fe-day-sticker.jpg" alt="santa fe daytime sticker">
<p>3" circle sticker. Great for slapping on your water bottle, laptop, or whatever the heck else you want!</p>
<h2>Shiprock, NM - Daytime/Nighttime</h2>
<section id="photos">
  <img src="{{ site.baseurl }}/images/design/shiprock-day-sticker.jpg" alt="shiprock daytime sticker">
  <img src="{{ site.baseurl }}/images/design/shiprock-night-sticker.jpg" alt="shiprock nighttime sticker">
</section>
<p>3" circle sticker. Great for slapping on your water bottle, laptop, or whatever the heck else you want!</p>

<script>
function currentDiv(n) {
  showDivs(slideIndex = n);
}

function showDivs(n) {
  var i;
  var x = document.getElementsByClassName("mySlides");
  var dots = document.getElementsByClassName("demo");
  if (n > x.length) {slideIndex = 1}
  if (n < 1) {slideIndex = x.length}
  for (i = 0; i < x.length; i++) {
    x[i].style.display = "none";
  }
  for (i = 0; i < dots.length; i++) {
    dots[i].className = dots[i].className.replace(" w3-opacity-off", "");
  }
  x[slideIndex-1].style.display = "block";
  dots[slideIndex-1].className += " w3-opacity-off";
}
</script>