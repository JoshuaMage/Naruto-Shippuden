<script>
  import OpeningVid from "$lib/video/openingVid.mp4";
  import Dropdown from "$lib/dropdown.svelte";
  import Hokage from '../routes/hokage/+page.svelte'

  let teams = [
    "Hokages",
    "Team 7",
    "Team Minato",
    "Akatsuki",
    "The Sannin",
    "Team 10",
    "Sand Siblings",
    "Taka",
    "Team Guy",
    "Team 8",
    "Seven Swordsmen",
  ];

  // Duplicate the teams for infinite scroll effect
  let infiniteTeams = [...teams, ...teams];
</script>

<div class="flex flex-col">
  <div>
    <video
      autoplay
      muted
      loop
      playsinline
      class="w-full h-[800px] object-cover"
    >
      <source src={OpeningVid} type="video/mp4" />
    </video>

    <section class="absolute bottom-50 left-10 w-[700px] text-start z-20">
      <p class="text-black text-6xl font-bold font-[cursive]">Welcome Ninja!</p>
      <p class="text-black text-xl font-bold font-[cursive]">
        This site is your guide to the Naruto universe. From legendary teams to
        the most powerful characters, learn everything you need to become a true
        shinobi expert.
      </p>
    </section>
  </div>

  <div class="relative w-full overflow-hidden flex justify-center">
    <div class="scroll-viewport w-[100vw] max-w-[90%] overflow-hidden">
      <div style="border-top: 3px solid white; margin: 20px 0;"></div>
      <div class="flex justify-center items-center h-64 animate-scroll">
        {#each infiniteTeams as team, index}
          <h2
            class="item font-[curved] font-bold text-6xl whitespace-nowrap mx-4 text-center"
            style="min-width: 500px"
          >
            {team}
          </h2>
        {/each}
      </div>
      <div style="border-top: 1px solid white; margin: 20px 0;"></div>
    </div>
  </div>

  <div class="flex justify-center">
    <Hokage />
  </div>
</div>
