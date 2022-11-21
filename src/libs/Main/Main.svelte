<script>
  import SectionAbout from "./SectionAbout.svelte";
  import SectionHero from "./SectionHero.svelte";
  import SectionWorked from "./SectionWorked.svelte";
</script>

<main>
  <!-- Hero Section -->
  <SectionHero />
  <SectionAbout />
  <SectionWorked />
</main>

<style lang="scss">
  main {
    margin: 0px auto;
    width: 100%;
    max-width: 1600px;
    min-height: 100vh;
    transition: all 200ms ease-in-out;
    padding: 0 25px;
    counter-reset: section 0;

    @media (min-width: 768px) {
      padding: 0px 140px;
    }
  }
</style>
