<script>
</script>

<div class="alert-popup">
  <p>En construction 🚧</p>
</div>

<style lang="scss">
  .alert-popup {
    display: flex;
    max-width: 300px;
    left: 10%;
    gap: 1em;
    border: 1px solid var(--green);
    padding: 1rem;
    border-radius: 4px;
    color: #ccd6f6;
    animation: slideIn 1s;
    animation-fill-mode: forwards;

    @keyframes slideIn {
      from {
        transform: translateY(-100px);
        opacity: 0;
      }
      to {
        transform: translateY(10%);
        opacity: 1;
      }
    }
  }
</style>
