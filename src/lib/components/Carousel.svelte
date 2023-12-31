<script>
    import Carousel from 'svelte-carousel';
    import { browser } from '$app/environment';
    import Industry from './news.svelte';
    import Heading from './Heading.svelte';
    let carousel; // for calling methods of the carousel instance
  const images = [
    "logo-1.png",
    "logo-2.png",
    "logo-3.png",
    "logo-4.png",
    "logo-5.png",
    "logo-6.png",
  ];
</script>
<div>
      {#if browser}
        <Carousel
          autoplay
          autoplayDuration={1000}
          particlesToShow={6}
          dots={false}
          arrows={false}
          bind:this={carousel}
          class="flex"
        >
          {#each images as imag}
            <div class="flex-shrink-0 bg-[#DAE6F2] py-24">
              <img src={imag} alt="" class="space-x-6 w-32" />
            </div>
          {/each}
        </Carousel>
      {/if}
    </div>