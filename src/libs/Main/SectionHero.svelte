<script>
  import Button from "../Global/Button.svelte";
</script>

<section class="hero-section">
  <h1>Hey👋, je me présente</h1>
  <h2>Dylan Jansana.</h2>
  <h3>Développeur web front-end.</h3>
  <p>
    Développeur web junior spécialisé dans l'intégration et l'interaction
    utilisateur. Je me concentre actuellement sur le développement de <a
      class="a"
      href="https://jolssy.xyz/">Jolssy</a
    >
    , je reste disponible pour toutes demandes.
  </p>
  <div>
    <Button size="xl" text="Mon github" />
  </div>
</section>

<style lang="scss">
  .hero-section {
    display: flex;
    flex-direction: column;
    max-width: 64rem /* 1024px */;
    min-height: calc(100vh - 300px);
    padding-top: 50%;
    margin: 0 auto;
    font-family: sans-serif;

    @media (min-width: 768px) {
      justify-content: center;
      padding-top: 0;
    }

    h1 {
      font-size: 1rem /* 16px */;
      line-height: 1.5rem /* 24px */;
      color: #64ffda;
      margin-left: 0.25rem /* 4px */;
      margin-bottom: 0.5rem /* 8px */;
      font-family: SF Mono Regular;
      @media (min-width: 768px) {
        margin-bottom: 1.5rem /* 24px */;
      }
    }

    h2 {
      font-size: 2.25rem /* 36px */;
      line-height: 2.5rem /* 40px */;
      color: #ccd6f6;
      font-weight: 600;
      line-height: 1.5;
      margin-bottom: 0.5rem /* 8px */;
      @media (min-width: 768px) {
        font-size: 4.5rem /* 72px */;
        line-height: 1;
        margin-bottom: 1rem /* 16px */;
      }
    }

    h3 {
      font-size: 1.875rem /* 30px */;
      line-height: 2.25rem /* 36px */;
      color: #8892b0;
      font-weight: 600;
      @media (min-width: 768px) {
        font-size: 3.75rem /* 60px */;
        line-height: 1;
      }
    }

    p {
      max-width: 540px;
      font-size: 1rem /* 16px */;
      line-height: 1.5rem /* 24px */;
      color: #8892b0;
      margin-top: 1.25rem /* 20px */;
      margin-bottom: 1rem /* 16px */;
      padding-bottom: 1rem;
      line-height: 1.5rem /* 24px */;
      a {
        color: #64ffda;
      }
    }
  }
</style>
