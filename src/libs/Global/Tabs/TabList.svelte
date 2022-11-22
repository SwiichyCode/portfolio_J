<div class="tab-list">
  <slot />
</div>

<style lang="scss">
  .tab-list {
    display: flex;
    width: 100%;
    overflow: scroll;
    padding-bottom: 0.5em;

    @media screen and (min-width: 640px) {
      flex-direction: column;
      overflow: initial;
      max-width: 120px;
    }
  }
</style>
