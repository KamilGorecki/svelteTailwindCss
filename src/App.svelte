<script>
  import Router from "svelte-spa-router"
  import Header from "./components/Header.svelte"
  import Home from "./routes/Home.svelte"
  import NotFound from "./routes/NotFound.svelte"

  const routes = {
    "/": Home,
    "*": NotFound,
  }
</script>

<style>
</style>

<main>
  <Header />
  <Router {routes} />
</main>
