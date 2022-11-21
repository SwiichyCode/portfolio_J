<script>
  import Fa from "svelte-fa";
  import {
    faGithub,
    faInstagram,
    faTwitter,
    faLinkedin,
    faTwitch,
  } from "@fortawesome/free-brands-svg-icons";
</script>

<nav class="side-social">
  <ul>
    <li>
      <a
        href="https://github.com/SwiichyCode"
        aria-label="Github"
        target="_blank"
        rel="noreferrer"><Fa icon={faGithub} /></a
      >
    </li>
    <li>
      <a
        href="https://www.instagram.com/?hl=fr"
        aria-label="Instagram"
        target="_blank"
        rel="noreferrer"><Fa icon={faInstagram} /></a
      >
    </li>
    <li>
      <a
        href="https://twitter.com/SwiichyCode_"
        aria-label="Twitter"
        target="_blank"
        rel="noreferrer"><Fa icon={faTwitter} /></a
      >
    </li>
    <li>
      <a
        href="https://fr.linkedin.com/"
        aria-label="Linkedin"
        target="_blank"
        rel="noreferrer"><Fa icon={faLinkedin} /></a
      >
    </li>
    <li>
      <a
        href="https://www.twitch.tv/swiichy_"
        aria-label="Codepen"
        target="_blank"
        rel="noreferrer"><Fa icon={faTwitch} /></a
      >
    </li>
  </ul>
  <div class="line" />
</nav>

<style lang="scss">
  .side-social {
    position: fixed;
    bottom: 0;
    left: 2.9rem /* 64px */;
    display: none;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    gap: 1.5rem /* 24px */;
    font-size: 22px;
    color: #ccd6f6;

    @media (min-width: 768px) {
      display: flex;
    }

    ul {
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      color: #ccd6f6;
    }

    li {
      padding: 0.75rem /* 12px */;
    }

    .line {
      width: 1px;
      height: 90px;
      background-color: #a8b2d1;
    }

    a {
      color: #ccd6f6;

      &:hover {
        color: #64ffda;
      }
    }
  }
</style>
