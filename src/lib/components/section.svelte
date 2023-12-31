<script>
    export let title;
    export let image;
    export let type = 'regular'; // Default to regular item
  </script>
  
  <div
    class="h-[500px] w-[370px] rounded-md {type === 'regular' ? 'pt-4' : ''} bg-white text-center space-y-5"
  >
    {#if type === 'regular'}
      <h1 class="text-[#01126C] hover:text-[#0A7BC9] text-2xl font-semibold">{title}</h1>
      <p class="text-gray-700 px-9 text-lg">Sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat</p>
      <button class="text-sm font-semibold text-[#0A7BC9]">Read More <i class="fa-solid fa-arrow-right" /></button>
      <img class="w-[370px] h-[295px]" src="{image}" alt="{title}" />
    {:else}
      <img class="w-[370px] h-[295px]" src="{image}" alt="{title}" />
      <h1 class="text-[#01126C] text-2xl font-semibold hover:text-[#0A7BC9]">{title}</h1>
      <p class="text-gray-700 px-9 text-lg">Sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat</p>
      <button class="text-sm font-semibold text-[#0A7BC9]">Read More <i class="fa-solid fa-arrow-right" /></button>
    {/if}
  </div>
  