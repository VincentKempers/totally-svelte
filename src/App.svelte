<script>
  import { Router, Route, Link } from "svelte-routing";
  import Home from "./pages/Home.svelte";
  import About from "./pages/About.svelte";
  export let url = "";
</script>

<Router url="{url}">
    <nav class="navigation">
        <h1 class="title">vincent kempers</h1>
        <ul class="links">
            <li><Link to="/" class="navigation-link">Home</Link></li>
            <li><Link to="about" class="navigation-link">About</Link></li>
        </ul>
    </nav>
   <div>
     <Route path="about" component="{About}" />
     <Route path="/"><Home /></Route>
   </div>
 </Router>


 <style>
     .navigation {
         padding: 1rem 2rem;
     }

     .navigation {
         font-family: Raleway, monospace;
         font-weight: 800;
         color: #fff;
         display: flex;
         flex-direction: row;
         justify-content: space-between;
         align-items: center;
     }

     .title {
         color: var(--theme-font-color);
     }

     .links {
         list-style: none;
         display: flex;
         flex-direction: row;
         align-items: center;
     }

     .links > li {
        padding-right: .5rem;
     }
 </style>
