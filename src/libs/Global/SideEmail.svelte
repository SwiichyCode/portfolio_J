<div class="side-email">
  <a href="mailto: swiichycode@gmail.com">swiichycode@gmail.com</a>
  <div class="line" />
</div>

<style lang="scss">
  .side-email {
    position: fixed;
    bottom: 0;
    right: 2.9rem /* 64px */;
    display: none;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    font-size: 14px;
    color: #ccd6f6;

    @media (min-width: 768px) {
      display: flex;
    }
  }
  a {
    writing-mode: vertical-rl;
    padding: 24px 0;
    margin: 0.75rem 0;
    text-decoration-skip-ink: auto;
    font-family: SF Mono Light;
    color: #ccd6f6;

    &:hover {
      color: #64ffda;
    }
  }

  .line {
    width: 1px;
    height: 90px;
    background: #a8b2d1;
  }
</style>
