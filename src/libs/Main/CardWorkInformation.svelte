<script>
  export let data;

  const {
    header: { poste, entreprise, date },
  } = data;
</script>

<article>
  <header>
    <h3><span>{poste}</span> <span class="company">{entreprise}</span></h3>
    <p class="subtitle">{date}</p>
  </header>
  <ul>
    {#each data.body as text}
      <li>
        {text}
      </li>
    {/each}
  </ul>
</article>

<style lang="scss">
  article {
    max-width: 550px;
    animation: fadeIn 2s;
  }
  header {
    h3 {
      margin-bottom: 4px;
      font-size: var(--fz-xl);
      font-weight: 500;
      line-height: 1.3;
      color: var(--lightest-slate);
      .company {
        color: var(--green);
      }
    }
    .subtitle {
      margin-bottom: 25px;
      color: var(--light-slate);
      font-family: var(--font-mono);
      font-size: var(--fz-xs);
    }
  }

  ul {
    padding: 0px;
    margin: 0px;
    list-style: none;
    font-size: var(--fz-md);

    li {
      position: relative;
      padding-left: 30px;
      margin-bottom: 10px;
      line-height: 1.3;

      &::before {
        content: "▹";
        position: absolute;
        left: 0px;
        color: var(--green);
      }
    }
  }

  @keyframes fadeIn {
    0% {
      opacity: 0;
    }
    100% {
      opacity: 1;
    }
  }
</style>
