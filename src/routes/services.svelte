<script>
  import Carousel from "../components/Carousel.svelte";
  import Panel from "../components/Panel.svelte";
  import Price from "../components/Pricing.svelte";
  import Mentenance from "../components/Mentenance.svelte";
  import Logodesign from "../components/Logodesign.svelte";

  let group = "Item ";
  let name = "world";
</script>

<style>
  h1 {
    text-align: center;
    margin-top: 20px;
  }

  h3 {
    text-align: center;
    margin: 20px;
  }

  p {
    margin: 10px;
    font-size: 22px;
    font-family: "eurostile", sans-serif;
    font-weight: 300;
    text-align: center;
  }

  .card {
    margin-top: 30px;
    margin-bottom: 30px;
    margin-left: auto;
    margin-right: auto;
    max-width: 750px;
    border-radius: 4px;
    box-shadow: 0 3px 3px -2px rgba(0, 0, 0, 0.2),
      0 3px 4px 0 rgba(0, 0, 0, 0.14), 0 1px 8px 0 rgba(0, 0, 0, 0.12);
    font-size: 14px;
  }

  .card a {
    display: inline-block;
    color: #e74c3c;
    text-decoration: none;
    border: 2px solid #e74c3c;
    border-radius: 24px;
    padding: 8px 20px;
    margin: 10px;
    transition: 0.4s linear;
    margin-bottom: 20px;
  }
  .card a:hover {
    color: #fff;
    background: #e74c3c;
  }
</style>

<svelte:head>
  <title>Service and Price</title>
  <meta
    name="description"
    content="Web Applications, Websites, Logos and Video Presentations" />
</svelte:head>

<h1>Latest Projects</h1>

<Carousel />
<h3>If you want to access the projects, just click on the table below</h3>
<div class="card">
  {#each Array(1) as _, i}
    <Panel name={`Websites | Web Apps`} bind:group>
      <div>
        <a href="https://www.pipemax.ro/" target="blank">Pipemax</a>
        <a href="https://viaengineering-development.com/" target="blank">
          ViaEngineering
        </a>
        <a href="https://websolver-calin.github.io/" target="blank">
          E-commerce
        </a>
        <a href="https://websolver.dev/weather/" target="blank">Weather App</a>

        <a href="https://websolver.dev/book-explorer/" target="blank">
          Books App
        </a>
        <a href="https://websolver.dev/Burger-app/" target="blank">
          Burger App
        </a>

        <a href="https://social-app-b9fc8.web.app/ " target="blank">
          Social App
        </a>
        <a href="https://websolver.dev/count-down/" target="blank">
          CountDown App
        </a>
      </div>
    </Panel>
  {/each}
</div>

<h1>Packages & Pricing</h1>
<p>
  From hosting and finding the right domain, to building websites and
  maintaining them everyday.
</p>
<Price />
<Mentenance />
<Logodesign />
