<script>
    import { onMount } from 'svelte';
  
    let isShaking = true;
    let buttonState = 'Stop';
    let headerOne;
    let intervalId;
  
    function getRandomHexColor() {
      const letters = '0123456789ABCDEF';
      let color = '#';
      for (let i = 0; i < 6; i++) {
        color += letters[Math.floor(Math.random() * 16)];
      }
      return color;
    }
  
    function stopShaking() {
      isShaking = !isShaking;
      buttonState = isShaking ? 'Stop' : 'Start';
  
      if (isShaking) {
        intervalId = setInterval(() => {
          headerOne.style.color = getRandomHexColor();
        }, 100);
      } else {
        clearInterval(intervalId);
      }
    }
  
    onMount(() => {
      if (isShaking) {
        intervalId = setInterval(() => {
          headerOne.style.color = getRandomHexColor();
        }, 100);
      }
    });
  </script>
  
  <section class="wrapper">
    <section class="part-1">
      <h1 class:crazy-shake={isShaking} bind:this={headerOne}>CRAZY</h1>
      <button on:click={stopShaking}>{buttonState} this shit</button>
    </section>
    <section class="part-2">
      <h2>BRUTAL</h2>
    </section>
    <section class="part-3">
      <h3 class="top-text">RIFT?</h3>
      <h3 class="bottom-text">RIFT?</h3>
    </section>
  </section>
  
  <style>
    /* ANIMATION CLASSES */
    .crazy-shake {
      animation: crazy-shake 0.1s linear infinite;
    }
  
    h1 {
      position: relative;
      font-family: 'Oswald', sans-serif;
      font-weight: 900;
      font-size: 150px;
      transform: rotate(-90deg);
      color: black;
    }
  
    h2 {
      font-family: 'Paytone One', sans-serif;
      color: black;
      font-size: 200px;
    }
  
    h3 {
      position: absolute;
      font-family: 'Paytone One', sans-serif;
      color: black;
      font-size: 150px;
    }

    .bottom-text:hover{
      animation: rip-text-upwards 1s forwards;
    }

    .bottom-text:hover .top-text{
      animation: rip-text-downwards 1s forwards;
    } 

    @keyframes rip-text-upwards{
      from{
        transform: translateY(0px);
        opacity: 1;
      }

      to{
        transform: translateY(-50px);
        opacity: 0.1;
      }
    }

    @keyframes rip-text-downwards{
      from{
        transform: translateY(0px);
      }

      to{
        transform: translateY(50px);
      }
    }

    .wrapper {
      background-color: black;
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      grid-template-rows: repeat(5, 1fr);
      grid-column-gap: 20px;
      grid-row-gap: 20px;
      height: 100dvh;
    }
  
    .part-1,
    .part-2,
    .part-3 {
      background-color: white;
      display: flex;
      justify-content: center;
      align-items: center;
    }
  
    .part-1 {
      grid-area: 1 / 1 / 6 / 2;
      flex-direction: column;
    }
  
    .part-1 button {
      position: absolute;
      bottom: 10%;
    }

    .part-3{
      position: relative;
      display: flex;
    }
  
    @keyframes crazy-shake {
      0% {
        transform: translateX(0px) translateY(0px) rotate(-90deg);
        /* font-variation-settings: "wght" 400; */
      }
      50% {
        transform: translateX(-20px) translateY(-20px) rotate(-90deg);
        /* font-variation-settings: "wght" 900; */
      }
    }
  
    .part-2 {
      grid-area: 1 / 2 / 4 / 4;
    }
  
    .part-3 {
      grid-area: 4 / 2 / 6 / 4;
    }
  </style>