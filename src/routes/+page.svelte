<script>
  import { Icon, Phone } from "svelte-hero-icons";
  import blueHeart from "$lib/img/blue-heart.jpg";
  import diamonds from "$lib/img/diamonds.jpg";
  import dolphin from "$lib/img/dolphin.jpg";
  import flower from "$lib/img/flower.jpg";
  import fullMoonDrops from "$lib/img/full-moon-drops.jpg";
  import rainbowDrops from "$lib/img/rainbow-drops.jpg";
  import blueNecklace from "$lib/img/blue-necklace.jpg";
  import orangeNecklace from "$lib/img/orange-necklace.jpg";
  import pinkNecklace from "$lib/img/pink-necklace.jpg";
  import unicorn from "$lib/img/unicorn.jpg";
  import beachHeart from "$lib/img/beach-heart.jpg";
  import hummingbirds from "$lib/img/hummingbirds.jpg";

  let exampleImages = [
    blueHeart,
    diamonds,
    dolphin,
    flower,
    fullMoonDrops,
    rainbowDrops,
    blueNecklace,
    orangeNecklace,
    pinkNecklace,
    unicorn,
    beachHeart,
    hummingbirds
  ];
</script>

<div class="hero min-h-[calc(100vh-150px)]">
  <div class="hero-overlay bg-opacity-60"></div>
  <div class="hero-content text-white text-center">
    <div class="max-w-md">
      <h1 class="mb-5 text-5xl font-bold pacifico">
        Welcome to High Sierra Mermaid
      </h1>
      <p class="mb-5">
        To view our current inventory, we invite you to call and schedule an
        appointment. Experience the charm and artistry of High Sierra Mermaid up
        close and personal.
      </p>
      <a href="tel:530-616-1754">
        <button class="btn bg-purple-950"
          ><Icon src={Phone} solid class="w-4 h-4 justify-self-end"></Icon>Call
          for Appointment</button
        >
      </a>
    </div>
  </div>
</div>

<!-- Examples Section -->
<div class=" h-full py-6 sm:py-8 lg:py-12">
  <div class="mx-auto max-w-screen-2xl px-4 md:px-8">
    <div class="flex items-center w-full mb-4">
      <h2 class="text-2xl font-bold lg:text-3xl mx-auto">Examples</h2>
    </div>
    <div class="text-center w-full mb-4 font-semibold">
      <p class="text-purple-950 mx-auto">
        Below are some examples of my previous work. Call or email for an
        appointment to see more.
      </p>
    </div>

    <div class="columns-xs gap-1">
      {#each exampleImages as image}
        <div class="m-4 sm:m-6">
          <a href={image} class="">
            <img
              src={image}
              loading="lazy"
              alt="Jewelry Example"
              class="rounded-2xl shadow-lg shadow-purple-950/50 hover:scale-110"
              target="_blank"
            />
          </a>
        </div>
      {/each}
    </div>
  </div>
</div>

<style>
  .hero {
    animation: slideshow 48s linear infinite;
  }

  @keyframes slideshow {
    0% {
      background-image: url("$lib/img/blue-heart.jpg");
    }
    20% {
      background-image: url("$lib/img/diamonds.jpg");
    }
    40% {
      background-image: url("$lib/img/dolphin.jpg");
    }
    60% {
      background-image: url("$lib/img/flower.jpg");
    }
    80% {
      background-image: url("$lib/img/full-moon-drops.jpg");
    }
    100% {
      background-image: url("$lib/img/rainbow-drops.jpg");
    }
  }
</style>
