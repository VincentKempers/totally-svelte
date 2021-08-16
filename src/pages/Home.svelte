<script>
  let pageName="Welcome to my page";
</script>

<main>
    <h1>Vincent Kempers</h1>
    <p>Welcome this is my <b>{pageName}</b></p>
    <div>
    <!-- Need to the get a new picture for my portfolio -->
        <!-- <img src="" alt="" /> -->
    </div>
</main>

<style>
  main {
      text-align: center;
      padding: 1em;
      max-width: 240px;
      margin: 0 auto;
      font-family: Raleway;
  }

  h1 {
      color: var(--main-font-color);
      text-transform: uppercase;
      letter-spacing: 22px;
      text-align: left;
      font-size: 4em;
      font-weight: 100;
  }

  p {
      font-family: BiterItalic;
      font-style: italic;
      color: white;
  }

  @media (min-width: 640px) {
      main {
          max-width: none;
      }
  }
</style>