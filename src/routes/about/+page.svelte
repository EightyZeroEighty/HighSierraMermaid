<script>
  import oceanna from "$lib/img/oceanna.jpg";
  import display from "$lib/img/display.jpg";
  import venmoQr from "$lib/img/venmo-qr.jpg";
</script>

<div class="p-10">
  <h1 class="text-5xl text-center my-5 font-bold pacifico">My Bio</h1>
  <div class="grid grid-cols-1 gap-4 pt-5">
    <div class="max-w-prose col-span-2 text-xl place-self-center">
      <p class="mb-5">
        Welcome to my Full Moon Lagoon, a magical collection of heartfelt
        treasures. I'm Oceanna Williams, the sole innovator of High Sierra
        Mermaid in Quincy, California. I design hand beaded jewelry, crystal
        prisms, and decor for home and office spaces.
      </p>
      <p>
        My business focus is based on "Sacred Commerce". All of My designs are
        unique and affordable. Custom orders are my specialty for all occasions. <br
        />
        Visit The Full Moon Lagoon on site, by appointment only. <br />
        530-616-1754 or OceannaWilliams54@gmail.com
      </p>
    </div>
    <div class="grid grid-cols-3">
      <img
        src={oceanna}
        alt="Oceanna Williams, owner of High Sierra Mermaid"
        class=" mb-5 rounded-2xl w-60 max-h-60"
      />

      <img
        src={display}
        alt="Exterior of the Full Moon Lagoon"
        class="rounded-2xl mb-5 w-60 max-h-64"
      />
      <img
        src={venmoQr}
        alt="Exterior of the Full Moon Lagoon"
        class="rounded-2xl w-60 max-h-64"
      />
    </div>
    <div class="grid mx-auto mt-5 col-span-full">
      <iframe
        class="mx-auto rounded-lg"
        width="560"
        height="315"
        src="https://www.youtube.com/embed/pLuiBZpSa1M?si=5f7E_2yRDwF5NVRL"
        title="YouTube video player"
        frameborder="0"
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
        referrerpolicy="strict-origin-when-cross-origin"
        allowfullscreen
      ></iframe>
    </div>
  </div>
</div>
