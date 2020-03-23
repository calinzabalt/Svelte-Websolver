<style>
  .card-container {
    margin-left: auto;
    margin-right: auto;
    text-align: center;
    display: flex;
    justify-content: center;
  }

  @media screen and (max-width: 600px) {
    .card-container {
      width: 100%;
      display: block;
      margin-bottom: 20px;
    }
  }

  .card {
    box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
    transition: 0.3s;
    max-width: 500px;
    display: inline-block;
    margin: 20px;
    margin-bottom: 40px;
  }

  .card:hover {
    box-shadow: 0 8px 16px 0 rgba(0, 0, 0, 0.2);
  }

  .container {
    padding: 2px 16px;
  }

  h4 {
    margin-top: 20px;
  }

  .card a {
    display: inline-block;
    color: #e74c3c;
    text-decoration: none;
    border: 2px solid #e74c3c;
    border-radius: 24px;
    padding: 8px 40px;
    transition: 0.4s linear;
    margin-bottom: 20px;
  }
  .card a:hover {
    color: #fff;
    background: #e74c3c;
  }

  h1 {
    text-align: center;
    padding-top: 20px;
    color: #293347;
  }
</style>

<svelte:head>
  <title>What's new ?</title>
  <meta name="description" content="What's new in web development ?" />
</svelte:head>

<h1>News</h1>
<div class="card-container">
  <div class="card">
    <img src="office.jpg" alt="img" style="width:100%;" />
    <div class="container">
      <h4>
        <b>Mobile-first indexing</b>
      </h4>
      <p>
        It's been a few years now that Google started working on mobile-first
        indexing - Google's crawling of the web using a smartphone Googlebot.
        From our analysis, most sites shown in search results are good to go for
        mobile-first indexing...
      </p>
      <a
        target="blank"
        href="https://webmasters.googleblog.com/2020/03/announcing-mobile-first-indexing-for.html">
        Read more
      </a>
    </div>
  </div>

  <div class="card">
    <img src="benefit.jpg" alt="img" style="width:100%" />
    <div class="container">
      <h4>
        <b>Benefits of owning a website</b>
      </h4>
      <p>
        Your website is a powerful marketing tool. Developing your web site
        offers many benefits including helping you get more leads and prospects,
        increase sales, enhance your professional brand, and improve your
        customer service.
      </p>
      <a
        target="blank"
        href="https://www.ecotonedigital.com/content-marketing/18-benefits-of-a-website-for-small-businesses/">
        Read more
      </a>
    </div>
  </div>
</div>
