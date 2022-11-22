<div class="alert-popup">
  <p>En construction 🚧</p>
</div>

<style lang="scss">
  .alert-popup {
    position: absolute;
    top: 10%;
    right: 5%;
    display: flex;
    max-width: 300px;
    gap: 1em;
    border: 1px solid var(--green);
    padding: 1rem;
    border-radius: 4px;
    color: #ccd6f6;
    animation: slideIn 1s;
    animation-fill-mode: forwards;

    @keyframes slideIn {
      from {
        transform: translateX(100px);
        opacity: 0;
      }
      to {
        transform: translateX(15%);
        opacity: 1;
      }
    }
  }
</style>
