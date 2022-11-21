<script>
  import Button from "../Global/Button.svelte";

  const items = [
    { text: "Présentation", href: "#" },
    { text: "Experience", href: "#" },
    { text: "Projet", href: "#" },
    { text: "Contact", href: "#" },
  ];
</script>

<nav>
  <ul class="header-nav">
    {#each items as { text, href }, index}
      <li class="nav-list">
        <a {href} class="flex items-center "
          ><span class="nav-index">0{index + 1}.</span>
          <span class="nav-text">{text}</span>
        </a>
      </li>
    {/each}
    <li>
      <Button text="C.V" />
    </li>
  </ul>
</nav>

<style lang="scss">
  .header-nav {
    display: none;
    align-items: center;
    gap: 2rem;
    font-size: 0.875rem;
    line-height: 1.25rem;
    color: #ccd6f6;
    font-family: SF Mono Light;

    @media (min-width: 768px) {
      display: flex;
    }

    .nav-index {
      color: #64ffda;
      padding-right: 0.25rem;
    }
    .nav-text {
      color: #b8c2e2;
    }
  }
  .nav-list:hover .nav-text {
    color: #64ffda;
    transition: all 200ms ease-in;
  }
  .nav-list:hover .nav-index {
    color: #ccd6f6;
    transition: all 200ms ease-in;
  }
</style>
