<script>
    import { onMount } from 'svelte';

    onMount(() => {
            let kaPow = document.querySelector('.kapow');

            //6 different sparkles
            let sparkles = [
                    "/images/sparkle1.png",
                    "/images/sparkle2.png",
                    "/images/sparkle3.png",
                    "/images/sparkle4.png",
                    "/images/sparkle5.png",
                    "/images/sparkle6.png",
                ]

            // 6 different pop-art images
            let popArtsImages = [
                "/images/popArtImage1.png",
                "/images/popArtImage2.png",
                "/images/popArtImage3.png",
                "/images/popArtImage4.png",
                "/images/popArtImage5.png",
                "/images/popArtImage6.png",
            ]
            
            // This function makes the "kapow" image follow the cursor, so when it's clicked it's in the right position.
            document.addEventListener('mousemove', (e) =>{
                kaPow.style.left = e.pageX + 'px';
                kaPow.style.top = e.pageY + 'px';
            })

            //This function makes the "kapow" image scale from 0 to 1, by adding a class.
            document.addEventListener('click', () => {
                kaPow.classList.add('kapowAnimation')
                kaPow.src = popArtsImages[Math.floor(Math.random() * popArtsImages.length)];
                document.addEventListener('animationend', () =>{
                    kaPow.classList.remove('kapowAnimation')
                })

            })

            //This function makes the sparkles follow the cursor.
            document.addEventListener('mousemove', (e) => {
                //set a randomnumber between -50 and 50
                let randomNumberX = Math.floor(Math.random() * 101) - 50;
                let randomNumberY = Math.floor(Math.random() * 101) - 50;


                //create a div
                let trailItem = document.createElement('div');

                //give the sparkle styling
                trailItem.className = 'trail-item';

                //set the position of the sparkle close to the cursor
                trailItem.style.top = e.pageY + randomNumberY + 'px';
                trailItem.style.left = e.pageX + randomNumberX + 'px';

                console.log(trailItem.style.top)

                //set the background to 1 of the 6 sparkles at random
                trailItem.style.background = "url(" + sparkles[Math.floor(Math.random() * sparkles.length)] + ")";
                trailItem.style.backgroundSize = "contain";
                
                //add the sparkles to the body
                document.body.appendChild(trailItem);
                
                //remove the sparkles after 2 seconds
                setTimeout(() => {
                    document.body.removeChild(trailItem)
                }, 2000)
            })
    })
</script>

<img src="/images/kapow.png" class="kapow" alt="kapow">

<style>

</style>