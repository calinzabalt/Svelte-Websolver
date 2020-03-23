<script>
  import Nav from "../components/Nav.svelte";
  import Fot from "../components/Footer.svelte";
  import GoogleAnalytics from "sapper-google-analytics/GoogleAnalytics.svelte";
  import { stores } from "@sapper/app";

  let ga_measurment_id = "UA-117582450-1"; // your analytics id

  export let segment;
</script>

<style>
  main {
    position: relative;
    background-color: white;
    margin: 0 auto;
    box-sizing: border-box;
  }
</style>

<GoogleAnalytics {stores} id={ga_measurment_id} />
<Nav {segment} />

<main>
  <slot />
</main>

<Fot />
