<script>
  export let text;
</script>

<button class="btn">
  {text}
</button>

<style>
  .btn {
    color: #64ffda;
    border: solid 1px #64ffda;
    font-family: SF Mono Light;
    padding: 10px 14px;
    border-radius: 0.25rem /* 4px */;
    background: transparent;
    cursor: pointer;
  }
  .btn:hover {
    background-color: rgba(100, 255, 218, 0.1);
    transition: all 0.25s cubic-bezier(0.645, 0.045, 0.355, 1);
  }
</style>
