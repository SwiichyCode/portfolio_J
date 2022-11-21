<section class="about-me global-section" data-sr-id="1">
  <header>
    <h2>À propos</h2>
    <div class="line" />
  </header>
  <div class="box">
    <p>
      Hello! My name is Dylan and I enjoy creating things that live on the
      internet. My interest in web development started back in 2012 when I
      decided to try editing custom Tumblr themes — turns out hacking together a
      custom reblog button taught me a lot about HTML & CSS!
    </p>
    <p>
      Fast-forward to today, and I’ve had the privilege of working at an
      advertising agency, a start-up, a huge corporation, and a student-led
      design studio. My main focus these days is building accessible, inclusive
      products and digital experiences at Upstatement for a variety of clients.
    </p>

    <p>
      I also recently launched a course that covers everything you need to build
      a web app with the Spotify API using Node & React.
    </p>

    <p>Here are a few technologies I’ve been working with recently:</p>
  </div>

  <ul>
    <li>JavaScript (ES6+)</li>
    <li>React</li>
    <li>Svelte</li>
    <li>Styled-components</li>
    <li>TypeScript</li>
    <li>Preact</li>
  </ul>
</section>

<style lang="scss">
  .about-me {
    margin-left: 20%;
    .box {
      max-width: 65%;
    }
    p {
      margin-bottom: 15px;
    }
    ul {
      display: grid;
      grid-template-columns: repeat(2, minmax(140px, 200px));
      gap: 0px 10px;
      padding: 0px;
      margin: 20px 0px 0px;
      overflow: hidden;
      list-style: none;

      li {
        position: relative;
        margin-bottom: 10px;
        padding-left: 20px;
        font-family: var(--font-mono);
        font-size: var(--fz-sm);
        font-family: "SF Mono Regular";

        &::before {
          content: "▹";
          position: absolute;
          left: 0px;
          color: var(--green);
          font-size: var(--fz-sm);
          line-height: 12px;
        }
      }
    }
  }
</style>
