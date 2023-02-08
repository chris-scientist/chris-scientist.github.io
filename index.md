---
layout: index
permalink: /
---

<header>
	<h1>
		chris-scientist studio
	</h1>
</header>
<section>
	<p class="comment" >// En (re)construction, revenez plus tard <span id="loading-text" data-index-anim="2" >!</span></p>
</section>
<section id="networks-global-container" >
	<h2>Réseaux :</h2>
	<ul class="networks-container" >
		<li class="network-container bg-twitter" >
			<ul>
				<li>Twitter</li>
				<li><a href="https://twitter.com/chr1ssc13nt1st" >@chr1ssc13nt1st</a></li>
			</ul>
		</li>
		<li class="network-container bg-instagram" >
			<ul>
				<li>Instagram</li>
				<li><a href="https://www.instagram.com/chr1ssc13nt1st/" >@chr1ssc13nt1st</a></li>
			</ul>
		</li>
		<li class="network-container bg-discord" >
			<ul>
				<li>Discord</li>
				<li><a href="javascript:void(0);" >chris-scientist#3276</a></li>
			</ul>
		</li>
	</ul>
</section>
<footer>
	<p>© {{ site.time | date: "%Y" }} - chris-scientist</p>
</footer>
<script text="text/javascript" >
	/* Animation du texte */
	setInterval(function() {
		var sequence = ['!', '/', '-', '\\', '|', '/', '-', '\\'];
		var index = $('#loading-text').data('index-anim');
		if(index < sequence.length) {
			index++;
		} else {
			index = 0;
		}
		$('#loading-text').text(sequence[index]);
		$('#loading-text').data('index-anim', index);
	}, 500);
</script>
