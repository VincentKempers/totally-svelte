<script>
  let pageName="Welcome to my page";
</script>

<main>
  <h1>{pageName}</h1>
  <p>Welcome this is my <b>{pageName}</b></p>
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
      color: #ff3e00;
      text-transform: uppercase;
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