---
title: "Contact"
weight: 50
draft: true
---
Une remarque, une question? Vous pouvez utiliser le formulaire ci-dessous, m'envoyer un email à lucie.descamps[@]ntnu.no, ou me retrouver sur Twitter.

<form id="contactform" method="post" action="https://formspree.io/insert.your@mail.adress">
	<div class="field half first">
		<input type="text" name="name" id="name" placeholder="Nom"/>
	</div>
	<div class="field half">
		<input type="email" id="email" name="email" placeholder="Email">
	</div>
	<div class="field">
		<textarea name="message" id="message" rows="4" placeholder="Message"></textarea>
	</div>
	<ul class="actions">
		<li><input type="submit" value="Envoyer" class="special" /></li>
		<li><input type="reset" value="Annuler" /></li>
	</ul>
	<input type="hidden" name="_next" value="?sent#formspree" />
	<input type="hidden" name="_subject" value="Subject for your mail like new message" />
	<input type="text" name="_gotcha" style="display:none" />
</form>
<span id="contactformsent">Merci pour votre message!</span>

<script>
$(document).ready(function($) {
    $(function(){
        if (window.location.search == "?sent") {
        	$('#contactform').hide();
        	$('#contactformsent').show();
        } else {
        	$('#contactformsent').hide();
        }
    });
});
</script>


{{< socialLinks >}}
