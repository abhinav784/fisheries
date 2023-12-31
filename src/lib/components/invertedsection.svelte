<!-- InvertedSection.svelte -->
<script>
    export let title;
    export let subtitle;
    export let description;
    export let items = [];
  </script>
  
  <div class="bg-blue-200">
    <h1 class="text-center text-blue-700 font-semibold text-xl pt-32">{title}</h1>
    <h2 class="text-4xl font-bold text-center text-blue-900 py-6">{subtitle}</h2>
    <p class="text-center text-gray-700 pb-7 text-lg px-8">{description}</p>
    <div class="flex justify-center space-x-4">
      {#each items as item (item.id)}
        <div class="bg-white w-[370px] h-[500px] rounded-md pt-4 text-center space-y-5">
          <h1 class="text-blue-900 hover:text-blue-700 text-2xl font-semibold">{item.title}</h1>
          <p class="text-gray-700 px-6 text-lg">{item.description}</p>
          <button class="text-sm font-semibold text-blue-700">Read More <i class="fa-solid fa-arrow-right" /></button>
          <img class="w-[370px] h-[295px]" src={item.imageUrl} alt={item.title} />
        </div>
      {/each}
    </div>
  </div>
  