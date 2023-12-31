<!-- OverlayBox.svelte -->
<script>
  export let items = [
    {
      image: "certificate.png",
      title: "Certified Farm",
      description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit.",
    },
    {
      image: "fish.png",
      title: "Organic Fish",
      description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit.",
    },
    {
      image: "quality.png",
      title: "High Quality",
      description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit.",
    },
  ];
</script>

<div class="bg-[#E4EBF5] hii z-20" name="box">
  <div class="rounded-xl mx-auto bg-[#CFE1F5] md:py-16 mb-10 w-[1150px] px-10">
    <div class="flex flex-col md:flex-row h-auto md:h-24">
      {#each items as { title, description, image }}
        <div
          class="text-center w-full md:w-1/3 (index === 2 ? 'border-white' : 'border-b md:border-b-0 md:border-r') border-b md:border-r border-white flex items-center justify-center"
        >
          <img src={image} alt={title} class="h-12 md:h-16 lg:h-20 mx-2" />
          <div>
            <div
              class="text-2xl md:text-3xl lg:text-4xl font-semibold text-[#01126C]"
            >
              {title}
            </div>
            <div class="text-sm md:text-base mt-1">{description}</div>
          </div>
        </div>
      {/each}
    </div>
  </div>
</div>

<style>
  .hii {
    position: absolute;
    top: 90%; /* Adjust as needed to position vertically */
    left: 50%;
    transform: translate(-50%, -50%);
    z-index: 2; /* Ensure it's above other elements */
  }
</style>
