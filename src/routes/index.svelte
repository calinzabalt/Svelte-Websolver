<script>
  import Sections from "../components/Sections.svelte";
  import Cards from "../components/Cards.svelte";
  import Sections2 from "../components/Sections2.svelte";
  let bgImage = "image.jpg";
</script>

<style>
  .pimg1 {
    position: relative;
    opacity: 0.7;
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
    background-attachment: fixed;
  }

  .pimg1 {
    width: 100%;
    height: 500px;
  }

  .ptext {
    position: absolute;
    top: 50%;
    width: 100%;
    text-align: center;
    color: #000;
    font-size: 3vw;
    letter-spacing: 6px;
    text-transform: uppercase;
  }

  .ptext .border {
    background-color: #111;
    color: #fff;
    padding: 12px;
  }

  @media (max-width: 568px) {
    .pimg1 {
      background-attachment: scroll;
      height: 300px;
    }
  }
</style>

<svelte:head>
  <title>Web Services !</title>
  <meta
    name="description"
    content="Together we will build unique and creative brands that will get a
    lot of attention online" />
</svelte:head>

<div class="pimg1" style="background-image: url('{bgImage}')">
  <div class="ptext">
    <span class="border">Build Your "Brand"</span>
  </div>
</div>

<Sections />
<Cards />
<Sections2 />
