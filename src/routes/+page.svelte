<script>
  import Carousel from "svelte-carousel";
  import { browser } from "$app/environment";
  import Testimonial from "$lib/components/Testimonial.svelte";
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
  <!-- <div class=" container h-2000 bg-gradient-to-r from-cyan-500 to-blue-500"> -->
  <div class="relative bg-cover bg-[url(fish13.png)]">
    <!-- bg-cover bg-no-repeat url('/background.jpg') -->

    <nav class=" mx-40 bg-[#01126C] shadow-lg opacity-80 sticky">
      <div class="max-w-7xl mx-auto px-4">
        <div class="flex justify-between">
          <div class="flex">
            <a href="#" class="flex items-center py-8 px-2">
              <img class="h-8 w-auto mr-2" src="Logo.png" alt="Logo" />
              <!-- <span class="font-semibold text-white text-lg">AQUAFY</span> -->
            </a>
          </div>
          <div class="hidden md:flex items-center space-x-1">
            <a href="#" class="py-4 px-2 text-gray-300 hover:text-white">Home</a
            >
            <a href="#" class="py-4 px-2 text-gray-300 hover:text-white"
              >Pages</a
            >
            <a href="#" class="py-4 px-2 text-gray-300 hover:text-white">Shop</a
            >
            <a href="#" class="py-4 px-2 text-gray-300 hover:text-white">Blog</a
            >
            <a href="#" class="py-4 px-2 text-gray-300 hover:text-white"
              >Contact Us</a
            >
          </div>
          <div class="md:hidden flex items-center">
            <button class="mobile-menu-button">
              <svg class="h-6 w-6 fill-current text-white" viewBox="0 0 24 24">
                <!-- <path v-if="!showMenu" fill-rule="evenodd" clip-rule="evenodd" d="M3 6h18v2H3V6zm0 5h18v2H3v-2zm0 5h18v2H3v-2z"/>
                  <path v-else fill-rule="evenodd" clip-rule="evenodd" d="M5 5h14v14H5V5zm2 2v10h10V7H7z"/> -->
              </svg>
            </button>
          </div>
        </div>
      </div>

      <div class="md:hidden mobile-menu">
        <a
          href="#"
          class="block py-2 px-4 text-sm text-gray-300 hover:text-white">Home</a
        >
        <a
          href="#"
          class="block py-2 px-4 text-sm text-gray-300 hover:text-white"
          >Pages</a
        >
        <a
          href="#"
          class="block py-2 px-4 text-sm text-gray-300 hover:text-white">Shop</a
        >
        <a
          href="#"
          class="block py-2 px-4 text-sm text-gray-300 hover:text-white">Blog</a
        >
        <a
          href="#"
          class="block py-2 px-4 text-sm text-gray-300 hover:text-white"
          >Contact Us</a
        >
      </div>
    </nav>

    <div class="pt-40 pb-5 text-5xl">
      <h1 class="font-bold text-white text-center">Aqua Fish farming</h1>
      <h1 class="font-bold text-white text-center">For the Aqua Fish Lovers</h1>
    </div>
    <h6 class="text-white text-center">
      Consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut
    </h6>
    <h6 class="  text-white text-center">
      labore et dolore magna aliquyam erat, sed diam voluptua.
    </h6>

    <!-- Button  -->
    <div class="flex justify-center pt-10">
      <button
        class=" bg-[#0A7BC9] text-white py-4 text-sm font-semibold px-9 rounded-md hover:text-[#0A7BC9] hover:bg-white"
      >
        Shop Now <i class="fa fa-arrow-right" />
      </button>
      <i class="fa-regular fa-circle-play text-white px-5 text-5xl" />
    </div>

    <div class="pb-80" />

    <!-- Overlay Box -->
    <div
      class="rounded-lg w-[1150px] h-52 absolute -bottom-24 bg-[#CFE1F5] py-10 mx-28"
    >
      <!-- <div class="flex h-24">
                <div class="font-bold text-center w-1/3 border-r border-white">Certified Farm</div>
                <div class="font-bold text-center w-1/3 border-r border-white">Organic Fish</div>
                <div class="font-bold text-center w-1/3">High quality</div>
              </div>
               -->
      <div class="flex h-24">
        <div
          class="text-center w-1/3 border-r border-white flex items-center justify-center"
        >
          <img src="certificate.png" alt="Certficate" class="h-12 mr-2" />
          <div>
            <div class="text-2xl font-semibold text-[#01126C]">
              Certified Farm
            </div>
            <div class="text-sm mt-1">
              Lorem ipsum dolor sit amet,<br /> consectetur adipiscing elit.
            </div>
          </div>
        </div>
        <div
          class="text-center w-1/3 border-r border-white flex items-center justify-center"
        >
          <img src="fish.png" alt="organic fish" class="h-12 mr-2" />
          <div>
            <div class="text-2xl font-semibold text-[#01126C]">
              Organic Fish
            </div>
            <div class="text-sm mt-1">
              Lorem ipsum dolor sit amet, <br />consectetur adipiscing elit.
            </div>
          </div>
        </div>
        <div class="text-center w-1/3 flex items-center justify-center">
          <img src="quality.png" alt="quality" class="h-12 mr-2" />
          <div class="">
            <div class="text-2xl font-semibold text-[#01126C]">
              High quality
            </div>
            <div class="text-sm mt-1">
              Lorem ipsum dolor sit amet,<br /> consectetur adipiscing elit.
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>

  <div />

  <!-- <div class="relative bg-black">Hello
    <div class="absolute inset-0 z-10 bg-slate-600">Rudy</div>
    <div class="relative z-20 bg-yellow-200">San</div>
  </div> -->
  <div class="bg-[#E4EBF5] h-80" />
  <!-- new about us -->
  <div class="flex w-full bg-[#E4EBF5] pb-28">
    <div class="w-1/2 relative">
      <img class="rounded-r-2xl w-[480px]" src="fish7.jpg" alt="" />
      <img
        class="rounded-2xl w-[350] shadow-xl right-20 absolute shadow-gray-500 h-[450px] top-14"
        src="fish8.jpg"
        alt=""
      />
    </div>
    <div class="w-1/2 space-y-5">
      <h1 class="text-[#0A7BC9] font-semibold text-xl">ABOUT US ~</h1>
      <h2 class="text-[#01126C] text-5xl font-bold">
        We Make You Healthy With Aqua Fresh Fishes
      </h2>
      <p class="text-xl text-gray-600">
        Consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut
        labore et dolore magna aliquyam erat, sed diam voluptua.At vero eos et
        accusam et justo duo dolores et ea rebum.
      </p>
      <p class="text-xl text-gray-600">
        Stet clita gubergren, no sea takimata sanctus est Lorem ipsum dolor sit
        amet. Lorem ipsum dolor sit amet, consetetur sadipscing elitr.
      </p>
      <ul class="flex text-gray-700 text-xl">
        <li class="">
          <i class="fa-regular fa-circle-right text-[#0A7BC9]" /> The Seafood Distribution
        </li>
        <li>
          <i class="fa-regular fa-circle-right text-[#0A7BC9]" /> The Seafood Processing
        </li>
      </ul>
      <ul class="flex text-xl text-gray-700">
        <li>
          <i class="fa-regular fa-circle-right text-[#0A7BC9]" /> Aquaculture Production
        </li>
        <li>
          <i class="fa-regular fa-circle-right text-[#0A7BC9]" /> Import Export Seafood
        </li>
      </ul>
      <button
        class="rounded-md px-9 py-4 font-semibold text-white bg-[#0A7BC9] text-sm"
        >Learn More <i class="fa fa-arrow-right" /></button
      >
    </div>
  </div>
  <!-- our best services  -->
  <div class="bg-[#E3EAFD]">
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
        <h1 class="text-[#01126C] hover:text-[#0A7BC9] text-2xl font-semibold">
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
        <h1 class="text-[#01126C] text-2xl font-semibold hover:text-[#0A7BC9]">
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
        <h1 class="text-[#01126C] text-2xl hover:text-[#0A7BC9] font-semibold">
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
    <!-- second -->
    <div class="flex justify-center space-x-4 pt-4 pb-28">
      <div
        class="h-[500px] w-[370px] rounded-md pt-4 bg-white text-center space-y-5"
      >
        <h1 class="text-[#01126C] hover:text-[#0A7BC9] text-2xl font-semibold">
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
        <h1 class="text-[#01126C] text-2xl font-semibold hover:text-[#0A7BC9]">
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
        <h1 class="text-[#01126C] text-2xl hover:text-[#0A7BC9] font-semibold">
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
  </div>

  <!-- About  us ~ -->
  <div class="flex bg-[#E4EBF5] pb-24">
    <div class="w-1/2 mt-28">
      <div class="pl-24 space-y-5">
        <h1 class="text-[#0A7BC9] font-semibold text-xl">ABOUT US ~</h1>
        <h2 class="text-[#01126C] text-5xl font-bold">
          Complete Destination for Aqua Farming
        </h2>
        <p class="text-gray-600 pr-24">
          Consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut
          labore et dolore magna aliquyam erat, sed diam voluptua.
        </p>
        <ul class="flex space-x-7">
          <li class="text-[#0A7BC9] text-6xl font-bold">30K</li>
          <li class="font-semibold w-12 text-xl pr-20 text-gray-500">
            Trusted Clients
          </li>
          <li class="text-[#0A7BC9] text-6xl font-bold">950</li>
          <li class="font-semibold w-12 text-xl text-gray-500">
            Finished Projects
          </li>
        </ul>
        <ul class="flex space-x-7">
          <li class="text-[#0A7BC9] text-6xl font-bold">25+</li>
          <li class="font-semibold w-20 text-xl text-gray-500">
            Years of Experiences
          </li>
          <li class="text-[#0A7BC9] text-6xl -mr-10 font-bold">650</li>
          <li class="font-semibold w-32 text-xl text-gray-500">
            Visiting Aqua Farming
          </li>
        </ul>
        <p class="text-gray-600">
          At vero eos et accusam et justo duo dolores et ea rebum. Stet clita
          gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet.
          Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam
          nonumy eirmod.
        </p>

        <button
          class="rounded-md px-9 py-4 font-semibold text-white bg-[#0A7BC9] text-sm"
          >Learn More <i class="fa fa-arrow-right" /></button
        >
      </div>
    </div>
    <div class="w=1/2 mt-56">
      <img
        class="rounded-2xl w-96 h-96 absolute ml-40"
        src="fish2.jpg"
        alt=""
      />
      <img
        class="rounded-2xl w-80 h-80 ml-10 -top-16 relative"
        src="fish3.jpg"
        alt=""
      />
    </div>
  </div>
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
        name="Colin Robinson"
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
  <div class="bg-[#DAE6F2] space-y-4 pt-32">
    <h1 class="text-center text-[#0A7BC9] font-semibold text-xl">
      ~ NEWS & BLOG ~
    </h1>
    <h2 class="text-4xl font-bold text-center text-[#01126C]">
      Our Latest Top Activities
    </h2>
    <div class="flex space-x-5 justify-center pt-20">
      <div class="bg-white w-[360px] h-[580px] rounded-md px-5 pt-4">
        <div class="relative">
          <img src="fish4.jpg" class="w-80 relative" alt="img" />
          <button
            class="bg-[#0A7BC9] absolute bottom-3 hover:bg-white hover:text-[#0A7BC9] left-2 font-semibold text-white rounded-3xl px-4 py-1"
            >Aquarium tips</button
          >
        </div>
        <div
          class="inline-block relative bottom-6 left-40 rounded-md px-5 py-3 text-center bg-[#01126C] text-white font-semibold"
        >
          <p class="">August 7, 2022</p>
        </div>

        <h1 class="text-[#01126C] font-semibold text-xl">
          Now to Keep Your Fishing Tackle Best
        </h1>

        <p class="text-gray-600 text-lg py-3">
          At vero eos et accusam et justo duo dolores et ea rebum. Stet clita
          kasd gubergren, no sea takimatasanctus est Lorem ipsum dolor sit…
        </p>
        <button class="text-[#0A7BC9] font-semibold"
          >Read More <i class="fa-solid fa-arrow-right" /></button
        >
      </div>

      <div class="bg-white w-[360px] h-[580px] rounded-md px-5 pt-4">
        <div class="relative">
          <img src="fish5.jpg" class="w-80 relative" alt="img" />
          <button
            class="bg-[#0A7BC9] absolute bottom-3 hover:bg-white hover:text-[#0A7BC9] left-2 font-semibold text-white rounded-3xl px-4 py-1"
            >Aquarium Fish</button
          >
        </div>
        <div
          class="inline-block relative bottom-6 left-40 rounded-md px-5 py-3 text-center bg-[#01126C] text-white font-semibold"
        >
          <p class="">August 7, 2022</p>
        </div>

        <h1 class="text-[#01126C] font-semibold text-xl">
          Now to Keep Your Fishing Tackle Best
        </h1>

        <p class="text-gray-600 text-lg py-3">
          At vero eos et accusam et justo duo dolores et ea rebum. Stet clita
          kasd gubergren, no sea takimatasanctus est Lorem ipsum dolor sit…
        </p>
        <button class="text-[#0A7BC9] font-semibold"
          >Read More <i class="fa-solid fa-arrow-right" /></button
        >
      </div>
      <div class="bg-white w-[360px] h-[580px] rounded-md px-5 pt-4 mb-9">
        <div class="relative">
          <img src="fish6.jpg" class="w-80 relative" alt="img" />
          <button
            class="bg-[#0A7BC9] absolute bottom-3 hover:bg-white hover:text-[#0A7BC9] left-2 font-semibold text-white rounded-3xl px-4 py-1"
            >Company News</button
          >
        </div>
        <div
          class="inline-block relative bottom-6 left-40 rounded-md px-5 py-3 text-center bg-[#01126C] text-white font-semibold"
        >
          <p class="">August 7, 2022</p>
        </div>

        <h1 class="text-[#01126C] font-semibold text-xl">
          5 Best Tips When Buying a Fishing Pole
        </h1>

        <p class="text-gray-600 py-3 text-lg">
          At vero eos et accusam et justo duo dolores et ea rebum. Stet clita
          kasd gubergren, no sea takimatasanctus est Lorem ipsum dolor sit…
        </p>
        <button class="text-[#0A7BC9] font-semibold"
          >Read More <i class="fa-solid fa-arrow-right" /></button
        >
      </div>
    </div>
    <button
      class="bg-[#0A7BC9] ml-[570px] px-9 text-white rounded-md font-semibold py-3"
      >See More <i class="fa-solid fa-arrow-right" />
    </button>
  </div>
  <!-- carousell/////////////////////// -->
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
  <!-- footerd -->
  <footer
    class="bg-[#01126C] py-20 px-10 bg-blend-lighten flex justify-around z-0 align-bottom"
  >
    <div class="w-1/3 ml-5 -pr-40 space-x-1">
      <img src="Logo.png" alt="" class="w-32" />
      <p class="m-5 pr-3 text-gray-300 font-semibold">
        Consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut
        labore et dolore magna aliquyam erat.
      </p>
      <i class="fa-brands fa-square-facebook text-white text-2xl" />
      <i class="fa-brands fa-square-instagram text-white text-2xl" />
      <i class="fa-brands fa-square-youtube text-white text-2xl" />
    </div>
    <div class="space-y-3 w-1/3 text-gray-300 font-semibold">
      <p class="font-bold decoration-2 text-white text-2xl">Our Services</p>
      <li>About Us</li>
      <li>Prodcuts</li>
      <li>Blogs</li>
      <li>Conatct Us</li>
    </div>
    <div class="space-y-3 w-1/3 text-gray-300 font-semibold">
      <p class="font-bold decoration-2 text-white text-2xl">Our Services</p>
      <li>About Us</li>
      <li>Prodcuts</li>
      <li>Blogs</li>
      <li>Conatct Us</li>
    </div>
    <div class="space-y-4 w-1/3 text-white conainer object-right">
      <p class="font-bold decoration-2 text-white text-2xl">Reach Us</p>
      <ul class="space-y-3">
        <li class="flex space-x-3">
          <i class="fa-sharp fa-solid fa-location-dot pt-1" />
          <p>Office: 09.00 am - 10.00 pm</p>
        </li>
        <li class="flex space-x-2">
          <i class="fa-solid fa-square-envelope pt-1" />
          <p>business@tensax.com</p>
        </li>
        <li class="flex space-x-2">
          <i class="fa-solid fa-phone-volume pt-1" />
          <p>0(141)3542867</p>
        </li>
      </ul>
    </div>
  </footer>
</div>
