<script>
	import { onMount } from 'svelte';

	onMount(() => {
		const testBtn = document.querySelector('.testbtn');
		testBtn.addEventListener('click', () => {
			svg.classList.toggle('svg-hidden');
		});
		let svg = document.querySelector('svg');
		console.log(svg);
	});
</script>

<button class="testbtn">TEST</button>

<svg
	class="svg-hidden"
	width="218"
	height="200"
	viewBox="0 0 218 200"
	fill="none"
	xmlns="http://www.w3.org/2000/svg"
>
	<path
		d="M218 100C218 155.228 173.228 200 118 200C62.7715 200 18 155.228 18 100C18 44.7715 62.7715 0 118 0C173.228 0 218 44.7715 218 100Z"
		fill="yellow"
		stroke="black"
	/>
	<path
		d="M192 122.305C168.751 157.207 138.036 168.821 110.123 168.821C82.2094 168.821 52 130.477 52 122.304C52 114.132 86.5867 130.321 114.5 130.321C142.413 130.321 192 114.132 192 122.305Z"
		fill="blue"
		class="mouth"
	/>
	<ellipse cx="50.5" cy="118" rx="4.5" ry="10" fill="black" />
	<ellipse cx="193.5" cy="118" rx="4.5" ry="10" fill="black" />
	<ellipse cx="142" cy="70" rx="16" ry="34" fill="black" />
	<ellipse cx="93" cy="70" rx="16" ry="34" fill="black" />
	<path d="M49 120C67.1128 157.156 121.671 209.688 195 122.563" stroke="black" stroke-width="4" />
	<path
		d="M92.4341 127.826L88.2338 142.813L86.5461 125.936L89.8376 125.524L92.4341 127.826Z"
		fill="#FF0000"
		stroke="black"
	/>
	<path
		d="M102.953 130.224L100.153 145.006L98.5441 128.916L100.86 128.53L102.953 130.224Z"
		fill="#FF0000"
		stroke="black"
	/>
	<path
		d="M74.3753 123.963L69.6655 134.56L70.4493 122.929L72.8392 122.533L74.3753 123.963Z"
		fill="#FF0000"
		stroke="black"
	/>
	<path d="M109 135L102.643 172L106 174L109.643 172.5L109 135Z" fill="yellow" />
	<path d="M109 135L102.643 172L106 174L109.643 172.5L109 135Z" fill="#FF0000" />
	<path d="M109 135L102.643 172L106 174L109.643 172.5L109 135Z" fill="#FF0000" />
	<path d="M109 135L102.643 172L106 174L109.643 172.5L109 135Z" fill="#FF0000" />
	<path d="M109 135L102.643 172L106 174L109.643 172.5L109 135Z" stroke="black" />
	<path d="M82.2319 130.5L74 157L76 160.5H79L82.2319 130.5Z" fill="#FF0000" />
	<path d="M82.2319 130.5L74 157L76 160.5H79L82.2319 130.5Z" fill="#FF0000" />
	<path d="M82.2319 130.5L74 157L76 160.5H79L82.2319 130.5Z" fill="#FF0000" />
	<path d="M82.2319 130.5L74 157L76 160.5H79L82.2319 130.5Z" fill="#FF0000" />
	<path d="M82.2319 130.5L74 157L76 160.5H79L82.2319 130.5Z" stroke="black" />
	<path d="M92 148L85 166.031L87.5 168.5L90.2662 168L92 148Z" fill="white" />
	<path d="M92 148L85 166.031L87.5 168.5L90.2662 168L92 148Z" fill="white" />
	<path d="M92 148L85 166.031L87.5 168.5L90.2662 168L92 148Z" fill="white" />
	<path d="M92 148L85 166.031L87.5 168.5L90.2662 168L92 148Z" fill="white" />
	<path d="M92 148L85 166.031L87.5 168.5L90.2662 168L92 148Z" stroke="black" />
	<path d="M163 143.5L163 157.031L166 156.5L167.5 153.5L163 143.5Z" fill="white" />
	<path d="M163 143.5L163 157.031L166 156.5L167.5 153.5L163 143.5Z" fill="white" />
	<path d="M163 143.5L163 157.031L166 156.5L167.5 153.5L163 143.5Z" fill="white" />
	<path d="M163 143.5L163 157.031L166 156.5L167.5 153.5L163 143.5Z" fill="white" />
	<path d="M163 143.5L163 157.031L166 156.5L167.5 153.5L163 143.5Z" stroke="black" />
	<path d="M122.6 145L121 173L124.5 175L129 173L122.6 145Z" fill="#FF0000" />
	<path d="M122.6 145L121 173L124.5 175L129 173L122.6 145Z" fill="#FF0000" />
	<path d="M122.6 145L121 173L124.5 175L129 173L122.6 145Z" fill="#FF0000" />
	<path d="M122.6 145L121 173L124.5 175L129 173L122.6 145Z" fill="#FF0000" />
	<path d="M122.6 145L121 173L124.5 175L129 173L122.6 145Z" stroke="black" />
	<path d="M143.5 131L142 169L146 170L149 166.5L143.5 131Z" fill="#FF0000" />
	<path d="M143.5 131L142 169L146 170L149 166.5L143.5 131Z" fill="#FF0000" />
	<path d="M143.5 131L142 169L146 170L149 166.5L143.5 131Z" fill="#FF0000" />
	<path d="M143.5 131L142 169L146 170L149 166.5L143.5 131Z" fill="#FF0000" />
	<path d="M143.5 131L142 169L146 170L149 166.5L143.5 131Z" stroke="black" />
	<path
		d="M138.442 127.08L134.672 155.853L132.521 128.253L135.113 126.526L138.442 127.08Z"
		fill="#FF0000"
		stroke="black"
	/>
	<path
		d="M161.442 123.08L157.672 151.853L155.521 124.253L158.113 122.526L161.442 123.08Z"
		fill="#FF0000"
		stroke="black"
	/>
	<path
		d="M116.592 129H119.43L115.672 157.686L113.528 130.167L116.592 129Z"
		fill="#FF0000"
		stroke="black"
	/>
	<line x1="46.4206" y1="71.7296" x2="64.4206" y2="99.7296" stroke="black" />
	<line x1="0.5" y1="25" x2="0.5" y2="26" stroke="black" />
	<line x1="48.5149" y1="83.8787" x2="51.5149" y2="71.8787" stroke="black" />
	<line x1="51.5385" y1="89.8077" x2="56.5385" y2="77.8077" stroke="black" />
	<line x1="56.6464" y1="96.6464" x2="63.6464" y2="89.6464" stroke="black" />
	<ellipse cx="93" cy="69.5" rx="6" ry="11.5" fill="white" />
	<ellipse cx="142" cy="69.5" rx="6" ry="11.5" fill="white" />
</svg>

<style>
	svg {
		display: block;
	}
	/* 
	.svg-hidden {
		display: none;
	} */

	.mouth {
		fill: red;
		animation: open-mouth 2s linear;
	}

	@keyframes open-mouth {
		from {
			transform: scale(0);
		}

		to {
			transform: scale(1);
		}
	}
</style>
