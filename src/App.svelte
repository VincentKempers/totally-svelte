<script>
  import { Router, Route, Link } from "svelte-routing";
  import Home from "./pages/Home.svelte";
  import About from "./pages/About.svelte";
  export let url = "";
</script>

<Router url="{url}">
  <nav class="navigation">
     <Link class="navigation-link" to="/">Home</Link>
     <Link class="navigation-link" to="about">About</Link>
   </nav>
   <div>
     <Route path="about" component="{About}" />
     <!--for now the router just support case sensitive,
         one workaround colud be add two time the route
         Example.
        <Route path="About" component="{About}" />
     -->
     <Route path="/"><Home /></Route>
   </div>
 </Router>


 <style>
     @font-face {
        font-family: Raleway;
        font-style: normal;
        font-weight: 400;
        src: url('/fonts/Raleway-VariableFont_wght.ttf') format('truetype');
    }

    @font-face {
        font-family: RalewayItalic;
        font-style: italic;
        font-weight: 400;
        src: url('/fonts/Raleway-Italic-VariableFont_wght.ttf') format('truetype');
    }

    @font-face {
        font-family: Bitter;
        font-style: normal;
        font-weight: 400;
        src: url('/fonts/Raleway-VariableFont_wght.ttf') format('truetype');
    }

    @font-face {
        font-family: BitterItalic;
        font-style: italic;
        font-weight: 400;
        src: url('/fonts/Raleway-Italic-VariableFont_wght.ttf') format('truetype');
    }

     .navigation {
         background-color: rgba(255, 255, 255, .3);
         padding: 1rem 2rem;
     }

     .navigation-link {
         font-family: Raleway, monospace;
         font-weight: 800;
     }
 </style>
