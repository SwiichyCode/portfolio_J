<script>
  import CardWorkInformation from "../../Main/CardWorkInformation.svelte";
  import { Tabs, TabList, TabPanel, Tab } from "./tabs.js";
  import { workedStore } from "../../../store/workedStore";
  console.log(workedStore[0].body.length);

  const items = [
    "Upstatement",
    "Scout",
    "Apple",
    "Scout",
    "Starry",
    "MullenLowe",
  ];
</script>

<Tabs>
  <div class="tabs-container">
    <TabList>
      {#each items as text, i} <Tab>{text}</Tab>{/each}
    </TabList>

    <div class="tabs-result">
      {#each workedStore as data, i}
        <TabPanel>
          <CardWorkInformation {data} />
        </TabPanel>
      {/each}
    </div>
  </div>
</Tabs>

<style lang="scss">
  .tabs-container {
    display: flex;
    flex-direction: column;
    gap: 1rem;
    min-height: 350px;

    @media screen and (min-width: 640px) {
      flex-direction: initial;
    }
  }

  .tabs-result {
    margin: 10px 0 0 0;
  }
</style>
