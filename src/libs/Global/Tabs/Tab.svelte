<script>
  import { getContext } from "svelte";
  import { TABS } from "./Tabs.svelte";

  const tab = {};
  const { registerTab, selectTab, selectedTab } = getContext(TABS);

  registerTab(tab);
</script>

<button class:selected={$selectedTab === tab} on:click={() => selectTab(tab)}>
  <span><slot /></span>
</button>

<style lang="scss">
  button {
    border: none;
    text-decoration: none;
    text-decoration-skip-ink: auto;
    transition: var(--transition);
    display: flex;
    -moz-box-align: center;
    align-items: center;
    width: 100%;
    height: var(--tab-height);
    padding: 0px 20px 2px;
    border-top: 2px solid var(--lightest-navy);
    background-color: transparent;
    color: var(--slate);
    font-family: "SF Mono Regular";
    font-size: var(--fz-xs);
    text-align: left;
    white-space: nowrap;
    text-transform: capitalize;
    cursor: pointer;

    @media screen and (min-width: 640px) {
      border-top: none;
      border-left: 2px solid var(--slate);
    }

    &:hover {
      color: var(--green);
      background-color: var(--light-navy);
    }
  }

  .selected {
    border-top: 2px solid #64ffda;
    color: var(--green);
    background-color: var(--light-navy);

    @media screen and (min-width: 640px) {
      border-left: 2px solid #64ffda;
      border-top: none;
    }
  }
</style>
