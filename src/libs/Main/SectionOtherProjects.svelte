<section class="other-projects">
  <header>
    <h2>Other Noteworthy Projects</h2>
    <a href="/">view the archive</a>
  </header>
</section>

<style lang="scss">
  .other-projects {
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    max-width: 64rem;

    header {
      display: flex;
      align-items: center;
      flex-direction: column;
      gap: 1rem;

      h2 {
        display: flex;
        -moz-box-align: center;
        align-items: center;
        position: relative;
        width: 100%;
        white-space: nowrap;
        font-size: clamp(26px, 5vw, var(--fz-heading));
        font-family: "Calibre Regular";
        color: #ccd6f6;
        font-weight: 600;
      }

      a {
        display: inline-block;
        text-decoration: none;
        text-decoration-skip-ink: auto;
        position: relative;
        transition: var(--transition);
        color: var(--green);
        font-family: "SF Mono Regular";
        font-size: var(--fz-sm);
      }
    }
  }
</style>
