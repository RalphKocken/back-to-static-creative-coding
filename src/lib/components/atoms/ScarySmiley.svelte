<script>
	import {onMount} from 'svelte';
	
	onMount(() => {
		const testButton = document.querySelector('.testBTN');
		const svg = document.querySelector('svg');
		const teeth = document.querySelectorAll('.teeth');
		const pupils = document.querySelectorAll('.eye-small')
		const leftEye = document.querySelector('.eye-big-left');
		const rightEye = document.querySelector('.eye-big-right');
		const mouth = document.querySelector('.mouth');
		const main = document.querySelector('main')
		testButton.addEventListener('click', () => {
			svg.classList.add('svg-animation')
			setTimeout(()=>{
				teeth.forEach(tooth =>{
					tooth.classList.add('teeth-animation');
				});
				pupils.forEach(pupil =>{
					pupil.classList.add('eye-small-animation')
				});
				leftEye.classList.add('eye-big-left-animation');
				rightEye.classList.add('eye-big-right-animation');
				mouth.classList.add('mouth-animation')
			}, 2000) 
			
			setTimeout(()=>{
					window.location.href = "/tournaments/new"
			},3000)
		})
	})

</script>
<div class="overlay">
	<svg width="300" height="300" viewBox="0 0 700 700" fill="none" xmlns="http://www.w3.org/2000/svg">
		<circle  cx="350" cy="350" r="345" fill="#FFFF00" stroke="black" stroke-width="10"/>
		<ellipse class="eye-big-left" cx="250.523" cy="224.448" rx="50" ry="100" fill="black"/>
		<ellipse class="eye-big-right" cx="442.085" cy="224.448" rx="50" ry="100" fill="black"/>
		<ellipse cx="442.085" cy="228.989" rx="50" ry="7.77203" fill="black"/>
		<ellipse cx="250.523" cy="228.989" rx="50" ry="7.77203" fill="black"/>
		<circle class="eye-small" cx="250.523" cy="228.989" r="50" fill="white"/>
		<circle class="eye-small" cx="442.085" cy="228.989" r="50" fill="white"/>
		<ellipse class="eye-small" cx="250.523" cy="230.602" rx="10.0503" ry="11.8102" fill="#FF0000"/>
		<ellipse class="eye-small" cx="442.085" cy="228.989" rx="10.0503" ry="11.8102" fill="#FF0000"/>
		<path class="mouth" d="M650 368.57C650 382.377 515.685 393.57 350 393.57C184.315 393.57 50 382.377 50 368.57C50 354.763 184.315 343.57 350 343.57C515.685 343.57 650 354.763 650 368.57Z" fill="black"/>
		<path class="teeth" d="M178.813 415.128L168.535 606.149L178.813 613.359L189.966 607.952L178.813 415.128Z" fill="#FF0000"/>
		<path class="teeth" d="M178.813 415.128L168.535 606.149L178.813 613.359L189.966 607.952L178.813 415.128Z" fill="#FF0000"/>
		<path class="teeth" d="M178.813 415.128L168.535 606.149L178.813 613.359L189.966 607.952L178.813 415.128Z" fill="#FF0000"/>
		<path class="teeth" d="M178.813 415.128L168.535 606.149L178.813 613.359L189.966 607.952L178.813 415.128Z" fill="#FF0000"/>
		<path class="teeth" d="M250.652 444.607L236.266 622.795L246.544 630.036L257.697 624.605L250.652 444.607Z" fill="#FF0000"/>
		<path class="teeth" d="M250.652 444.607L236.266 622.795L246.544 630.036L257.697 624.605L250.652 444.607Z" fill="#FF0000"/>
		<path class="teeth" d="M250.652 444.607L236.266 622.795L246.544 630.036L257.697 624.605L250.652 444.607Z" fill="#FF0000"/>
		<path class="teeth" d="M250.652 444.607L236.266 622.795L246.544 630.036L257.697 624.605L250.652 444.607Z" fill="#FF0000"/>
		<path class="teeth" d="M335.325 376.606L324.369 630.228L335.325 638.186L345.8 632.014L335.325 376.606Z" fill="#FF0000"/>
		<path class="teeth" d="M335.325 376.606L324.369 630.228L335.325 638.186L345.8 632.014L335.325 376.606Z" fill="#FF0000"/>
		<path class="teeth" d="M335.325 376.606L324.369 630.228L335.325 638.186L345.8 632.014L335.325 376.606Z" fill="#FF0000"/>
		<path class="teeth" d="M335.325 376.606L324.369 630.228L335.325 638.186L345.8 632.014L335.325 376.606Z" fill="#FF0000"/>
		<path class="teeth" d="M425.737 400.6L430.257 622.606L445.375 627.887L454.955 613.838L425.737 400.6Z" fill="#FF0000"/>
		<path class="teeth" d="M425.737 400.6L430.257 622.606L445.375 627.887L454.955 613.838L425.737 400.6Z" fill="#FF0000"/>
		<path class="teeth" d="M425.737 400.6L430.257 622.606L445.375 627.887L454.955 613.838L425.737 400.6Z" fill="#FF0000"/>
		<path class="teeth" d="M425.737 400.6L430.257 622.606L445.375 627.887L454.955 613.838L425.737 400.6Z" fill="#FF0000"/>
		<path class="teeth" d="M510.442 462.801L518.568 611.842L530.08 603.815H541.345L510.442 462.801Z" fill="#FF0000"/>
		<path class="teeth" d="M510.442 462.801L518.568 611.842L530.08 603.815H541.345L510.442 462.801Z" fill="#FF0000"/>
		<path class="teeth" d="M510.442 462.801L518.568 611.842L530.08 603.815H541.345L510.442 462.801Z" fill="#FF0000"/>
		<path class="teeth" d="M510.442 462.801L518.568 611.842L530.08 603.815H541.345L510.442 462.801Z" fill="#FF0000"/>
		<path class="teeth" d="M380.152 627.887L390.43 376.115L380.152 362.573L368.999 372.73L380.152 627.887Z" fill="#FF0000"/>
		<path class="teeth" d="M380.152 627.887L390.43 376.115L380.152 362.573L368.999 372.73L380.152 627.887Z" fill="#FF0000"/>
		<path class="teeth" d="M380.152 627.887L390.43 376.115L380.152 362.573L368.999 372.73L380.152 627.887Z" fill="#FF0000"/>
		<path class="teeth" d="M380.152 627.887L390.43 376.115L380.152 362.573L368.999 372.73L380.152 627.887Z" fill="#FF0000"/>
		<path class="teeth" d="M295.045 627.887L311.727 375.93L301.449 362.544L290.296 372.584L295.045 627.887Z" fill="#FF0000"/>
		<path class="teeth" d="M295.045 627.887L311.727 375.93L301.449 362.544L290.296 372.584L295.045 627.887Z" fill="#FF0000"/>
		<path class="teeth" d="M295.045 627.887L311.727 375.93L301.449 362.544L290.296 372.584L295.045 627.887Z" fill="#FF0000"/>
		<path class="teeth" d="M295.045 627.887L311.727 375.93L301.449 362.544L290.296 372.584L295.045 627.887Z" fill="#FF0000"/>
		<path class="teeth" d="M219.461 604.742L229.74 383.396L219.461 371.129L208.309 380.33L219.461 604.742Z" fill="#FF0000"/>
		<path class="teeth" d="M219.461 604.742L229.74 383.396L219.461 371.129L208.309 380.33L219.461 604.742Z" fill="#FF0000"/>
		<path class="teeth" d="M219.461 604.742L229.74 383.396L219.461 371.129L208.309 380.33L219.461 604.742Z" fill="#FF0000"/>
		<path class="teeth" d="M219.461 604.742L229.74 383.396L219.461 371.129L208.309 380.33L219.461 604.742Z" fill="#FF0000"/>
		<path class="teeth" d="M482.912 581.917V379.242L472.633 372.279L461.48 377.501L482.912 581.917Z" fill="#FF0000"/>
		<path class="teeth" d="M482.912 581.917V379.242L472.633 372.279L461.48 377.501L482.912 581.917Z" fill="#FF0000"/>
		<path class="teeth" d="M482.912 581.917V379.242L472.633 372.279L461.48 377.501L482.912 581.917Z" fill="#FF0000"/>
		<path class="teeth" d="M482.912 581.917V379.242L472.633 372.279L461.48 377.501L482.912 581.917Z" fill="#FF0000"/>
		<path class="teeth" d="M564.545 547.4L585.976 413.759L575.698 406.796L564.545 412.018V547.4Z" fill="#FF0000"/>
		<path class="teeth" d="M564.545 547.4L585.976 413.759L575.698 406.796L564.545 412.018V547.4Z" fill="#FF0000"/>
		<path class="teeth" d="M564.545 547.4L585.976 413.759L575.698 406.796L564.545 412.018V547.4Z" fill="#FF0000"/>
		<path class="teeth" d="M564.545 547.4L585.976 413.759L575.698 406.796L564.545 412.018V547.4Z" fill="#FF0000"/>
		<path class="teeth" d="M146.528 563.155L150.692 399.726L140.414 395.546L129.261 398.681L146.528 563.155Z" fill="#FF0000"/>
		<path class="teeth" d="M146.528 563.155L150.692 399.726L140.414 395.546L129.261 398.681L146.528 563.155Z" fill="#FF0000"/>
		<path class="teeth" d="M146.528 563.155L150.692 399.726L140.414 395.546L129.261 398.681L146.528 563.155Z" fill="#FF0000"/>
		<path class="teeth" d="M146.528 563.155L150.692 399.726L140.414 395.546L129.261 398.681L146.528 563.155Z" fill="#FF0000"/>
		</svg>
		


</div>
	<style>
	</style>