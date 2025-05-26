<script>
  import Danzo from "$lib/hokage/hiddenLeaf/Danzo.jpg";
  import Hashirama from "$lib/hokage/hiddenLeaf/hashirama.jpg";
  import Hiruzen from "$lib/hokage/hiddenLeaf/Hiruzen.jpg";
  import Kakashi from "$lib/hokage/hiddenLeaf/Kakashi.jpg";
  import Minato from "$lib/hokage/hiddenLeaf/Minato.jpg";
  import Naruto from "$lib/hokage/hiddenLeaf/Naruto.jpg";
  import Shikamaru from "$lib/hokage/hiddenLeaf/Shikamaru.jpg";
  import Tobirama from "$lib/hokage/hiddenLeaf/Tobirama.jpg";
  import Tsuande from "$lib/hokage/hiddenLeaf/Tsunade.jpg";

  import Gaara from "$lib/hokage/hiddenSand/Gaara.jpg";
  import Rasa from "$lib/hokage/hiddenSand/Rasa.jpg";
  import Reto from "$lib/hokage/hiddenSand/Reto.jpg";
  import Shamon from "$lib/hokage/hiddenSand/Shamon.jpg";
  import Sunagakure from "$lib/hokage/hiddenSand/Sunagakure.jpg";

  import Byakuren from "$lib/hokage/hiddenMist/byakuren.jpg";
  import Chojuro from "$lib/hokage/hiddenMist/Chojuro.jpg";
  import Gengetsu from "$lib/hokage/hiddenMist/Gengetsu .jpg";
  import Mei from "$lib/hokage/hiddenMist/Mei.jpg";
  import Third from "$lib/hokage/hiddenMist/ThirdMizukage.jpg";
  import Yagura from "$lib/hokage/hiddenMist/Yagura.jpg";

  let hiddenHOkage = [
    { name: "First Hokage", image: Hashirama },
    { name: "Second Hokage", image: Tobirama },
    { name: "Third Hokage", image: Hiruzen },
    { name: "Fourth Hokage", image: Minato },
    { name: "Fifth Hokage", image: Tsuande },
    { name: "Temporary Sixth Hokage", image: Danzo },
    { name: "Sixth Hokage", image: Kakashi },
    { name: "Seventh Hokage", image: Naruto },
    { name: "Eighth Hokage", image: Shikamaru },
  ];

  let sandHokage = [
    { name: "First Kazekage", image: Reto },
    { name: "Second Kazekage", image: Shamon },
    { name: "Third Kazekage", image: Rasa },
    { name: "Fourth Kazekage", image: Sunagakure },
    { name: "Fifth Kazekage", image: Gaara },
  ];

  let mistdHokage = [
    { name: "First Mizukage", image: Byakuren },
    { name: "Second Mizukage", image: Gengetsu },
    { name: "Third Mizukage", image: Third },
    { name: "Fourth Mizukage", image: Yagura },
    { name: "Fifth Mizukage", image: Mei },
    { name: "Sixth Mizukage", image: Chojuro },
  ];
</script>

<div class="text-center">
  <h3 class="font-bold text-6xl pb-10">Hokage</h3>
  <div class="pb-10">
    <h4 class="font-bold text-2xl pb-10">Hidden Leaf Village Hokage's</h4>
    <div class="grid grid-cols-3 gap-10 m-10">
      {#each hiddenHOkage as hokage}
        <div class="relative group overflow-hidden">
          <img
            src={hokage.image}
            alt={hokage.name}
            class=" transition-transform duration-300 group-hover:scale-110 rounded-xl size-[500px]"
          />
          <div
            class="absolute inset-0 bg-black bg-opacity-50 flex items-center justify-center opacity-0 group-hover:opacity-50 transition-opacity duration-300"
          >
            <p class="text-white text-3xl font-bold">{hokage.name}</p>
          </div>
        </div>
      {/each}
    </div>
  </div>

  <div class="pb-10">
    <h4 class="font-bold text-2xl pb-10">Hidden Sand Village Hokage's</h4>
    <div class="grid grid-cols-3 gap-10 m-10">
      {#each sandHokage as hokage}
        <div class="relative group overflow-hidden">
          <img
            src={hokage.image}
            alt={hokage.name}
            class=" transition-transform duration-300 group-hover:scale-110 rounded-xl size-[500px]"
          />
          <div
            class="absolute inset-0 bg-black bg-opacity-50 flex items-center justify-center opacity-0 group-hover:opacity-50 transition-opacity duration-300"
          >
            <p class="text-white text-3xl font-bold">{hokage.name}</p>
          </div>
        </div>
      {/each}
    </div>
  </div>

  <div class="pb-10">
    <h4 class="font-bold text-2xl pb-10">Hidden Mist Village Hokage's</h4>
    <div class="grid grid-cols-3 gap-10 m-10">
      {#each mistdHokage as hokage}
        <div class="relative group overflow-hidden">
          <img
            src={hokage.image}
            alt={hokage.name}
            class=" transition-transform duration-300 group-hover:scale-110 rounded-xl size-[500px]"
          />
          <div
            class="absolute inset-0 bg-black bg-opacity-50 flex items-center justify-center opacity-0 group-hover:opacity-50 transition-opacity duration-300"
          >
            <p class="text-white text-3xl font-bold">{hokage.name}</p>
          </div>
        </div>
      {/each}
    </div>
  </div>
</div>
