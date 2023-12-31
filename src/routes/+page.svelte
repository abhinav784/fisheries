<script>
  import Carousel from "svelte-carousel";
  import { browser } from "$app/environment";
  import Testimonial from "$lib/components/Testimonial.svelte";
  import Heading from "../lib/components/Heading.svelte";
  import Footer from "../lib/components/Footer.svelte";
  import AiIndustries from "../lib/components/Carousel.svelte";
  import News from "../lib/components/news.svelte";
  import Hero from "../lib/components/Hero.svelte";
  import Howitworks from "../lib/components/How it works.svelte";
  import Aboutus from "../lib/components/Aboutus.svelte";
  import Section from "../lib/components/section.svelte";
  import Overlaybox from "../lib/components/overlaybox.svelte";
  import About from "../lib/components/About.svelte";
  const services = [
    { title: "Aquarium Fish", image: "fish11.png", type: "regular" },
    { title: "Aquatic Plant", image: "fish12.png", type: "inverted" },
    { title: "Hatchery Supply", image: "fish13.png", type: "regular" },
  ];
  const servicess = [
    { title: "Green Care", image: "fish14.png", type: "regular" },
    { title: "Prawn Feeds", image: "fish16.png", type: "inverted" },
    { title: "Flowerhorn Fish", image: "fish17.png", type: "regular" },
  ]; // Default to regular item
</script>

<!-- Navbar -->

<div>
  <!-- <div class=" container h-2000 bg-gradient-to-r from-cyan-500 to-blue-500"> -->
  <div
    class="relative"
    style="background-image:url(hero-bg.jpg); height:850px;"
  >
    <!-- bg-cover bg-no-repeat url('/background.jpg') -->
    <Heading />

    <Hero />

    <!-- our best services  -->
    <!-- <div class="bg-[#E3EAFD]">
      <h1 class="text-center text-[#0A7BC9] font-semibold text-xl pt-32">
        ~ OUR BEST SERVICES ~
      </h1>
      <h2 class="text-4xl font-bold text-center text-[#01126C] py-6">
        Fish Farming Start With Us
      </h2>
      <p
        class="
     text-center text-gray-700 pb-7 text-lg px-96"
      >
        Consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut
        labore et dolore magna aliquyam erat, sed diam voluptua.
      </p>
      <div class="flex justify-center space-x-4">
        <div
          class="h-[500px] w-[370px] rounded-md pt-4 bg-white text-center space-y-5"
        >
          <h1
            class="text-[#01126C] hover:text-[#0A7BC9] text-2xl font-semibold"
          >
            Aquarium Fish
          </h1>
          <p class="text-gray-700 px-9 text-lg">
            Sed diam nonumy eirmod tempor invidunt ut labore et dolore magna
            aliquyam erat
          </p>
          <button class="text-sm font-semibold text-[#0A7BC9]"
            >Read More <i class="fa-solid fa-arrow-right" /></button
          >
          <img class="w-[370px] h-[295px]" src="fish11.png" alt="" />
        </div>
        <div
          class="h-[510px] w-[370px] rounded-md bg-white text-center space-y-5"
        >
          <img class="w-[370px] h-[295px]" src="fish12.png" alt="" />
          <h1
            class="text-[#01126C] text-2xl font-semibold hover:text-[#0A7BC9]"
          >
            Aquatic Plant
          </h1>
          <p class="text-gray-700 px-9 text-lg">
            Sed diam nonumy eirmod tempor invidunt ut labore et dolore magna
            aliquyam erat
          </p>
          <button class="text-sm font-semibold text-[#0A7BC9]"
            >Read More <i class="fa-solid fa-arrow-right" /></button
          >
        </div>
        <div
          class="h-[500px] w-[370px] rounded-md pt-4 bg-white text-center space-y-5"
        >
          <h1
            class="text-[#01126C] text-2xl hover:text-[#0A7BC9] font-semibold"
          >
            Hatchery Supply
          </h1>
          <p class="text-gray-700 text-lg px-9">
            Sed diam nonumy eirmod tempor invidunt ut labore et dolore magna
            aliquyam erat
          </p>
          <button class="text-sm font-semibold text-[#0A7BC9]"
            >Read More <i class="fa-solid fa-arrow-right" /></button
          >
          <img class="w-[370px] h-[295px]" src="fish13.png" alt="" />
        </div>
      </div> 
      second
      <div class="flex justify-center space-x-4 pt-4 pb-28">
        <div
          class="h-[500px] w-[370px] rounded-md pt-4 bg-white text-center space-y-5"
        >
          <h1
            class="text-[#01126C] hover:text-[#0A7BC9] text-2xl font-semibold"
          >
            Green Care
          </h1>
          <p class="text-gray-700 px-9 text-lg">
            Sed diam nonumy eirmod tempor invidunt ut labore et dolore magna
            aliquyam erat
          </p>
          <button class="text-sm font-semibold text-[#0A7BC9]"
            >Read More <i class="fa-solid fa-arrow-right" /></button
          >
          <img class="w-[370px] h-[295px]" src="fish14.png" alt="" />
        </div>
        <div
          class="h-[510px] w-[370px] rounded-md bg-white text-center space-y-5"
        >
          <img class="w-[370px] h-[295px]" src="fish16.png" alt="" />
          <h1
            class="text-[#01126C] text-2xl font-semibold hover:text-[#0A7BC9]"
          >
            Prawn Feeds
          </h1>
          <p class="text-gray-700 px-9 text-lg">
            Sed diam nonumy eirmod tempor invidunt ut labore et dolore magna
            aliquyam erat
          </p>
          <button class="text-sm font-semibold text-[#0A7BC9]"
            >Read More <i class="fa-solid fa-arrow-right" /></button
          >
        </div>
        <div
          class="h-[500px] w-[370px] rounded-md pt-4 bg-white text-center space-y-5"
        >
          <h1
            class="text-[#01126C] text-2xl hover:text-[#0A7BC9] font-semibold"
          >
            Flowerhorn Fish
          </h1>
          <p class="text-gray-700 text-lg px-9">
            Sed diam nonumy eirmod tempor invidunt ut labore et dolore magna
            aliquyam erat
          </p>
          <button class="text-sm font-semibold text-[#0A7BC9]"
            >Read More <i class="fa-solid fa-arrow-right" /></button
          >
          <img class="w-[370px] h-[295px]" src="fish17.png" alt="" />
        </div>
      </div>
    </div> -->
    <Overlaybox />
    <About />
    <div class="bg-[#E3EAFD]">
      <h1 class="text-center text-[#0A7BC9] font-semibold text-xl pt-32">
        ~ OUR BEST SERVICES ~
      </h1>
      <h2 class="text-4xl font-bold text-center text-[#01126C] py-6">
        Fish Farming Start With Us
      </h2>
      <p class="text-center text-gray-700 pb-7 text-lg px-96">
        Consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut
        labore et dolore magna aliquyam erat, sed diam voluptua.
      </p>

      <div class="flex justify-center mb-4 space-x-4">
        {#each services as service}
          <Section {...service} />
        {/each}
      </div>
      <div class="flex justify-center mt-4 space-x-4">
        {#each servicess as service}
          <Section {...service} />
        {/each}
      </div>
    </div>
    <!-- ~ About  us ~ -->
    <Aboutus />

    <!-- new section -->
    <Howitworks />

    <!-- What our client say -->

    <div class="bg-[#D8E5F1] bg-[url(testimonial-bg.png)">
      <h1 class=" text-[#0A7BC9] font-semibold text-xl pt-32 pl-28">
        TESTIMONIAL ~
      </h1>
      <div class="flex">
        <h2 class="text-4xl font-bold text-[#01126C] py-6 pl-28 w-1/2">
          See, What Our Client Say
        </h2>
        <p class=" text-gray-700 pb-7 text-lg w-1/2 pr-28">
          Consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut
          labore et dolore magna aliquyam erat, sed diam voluptua.
        </p>
      </div>
      <div class="flex justify-center space-x-4 pt-16">
        <Testimonial
          name="Colin Robinson"
          country="America"
          comment="Sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores"
          img="/dp55.png"
        />
        <Testimonial
          name="John Doe"
          country="America"
          comment="Sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores"
          img="/dp33.png"
        />
        <Testimonial
          name="rechaerd furi"
          country="America"
          comment="Sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores"
          img="/dp44.png"
        />
      </div>
    </div>

    <!-- news & blogs -->
    <News />
    <!-- carousell/////////////////////// -->
    <AiIndustries />
    <!-- footerd -->
    <Footer />
  </div>
</div>
