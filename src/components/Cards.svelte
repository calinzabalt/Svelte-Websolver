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
</style>

<div class="card-container">
  <div class="card">
    <img src="rsz_design.jpg" alt="img" style="width:100%;" />
    <div class="container">
      <h4>
        <b>Logo Design & Video Presentations</b>
      </h4>
      <p>
        Have you got bored of searching for web designers who can't create your
        logo or video presentation ? If so, then we have a solution for this. If
        we put our minds together, we can create unique logos and video
        presentations for your business.
      </p>
      <a href="contact">Contact</a>
    </div>
  </div>

  <div class="card">
    <img src="paper-on-gray-laptop-669617.jpg" alt="img" style="width:100%" />
    <div class="container">
      <h4>
        <b>Why to use a CRM ?</b>
      </h4>
      <p>
        A CRM can have a pretty big impact on your business, it will make your
        life a lot easier and it can increase your sales, leads, subscribers
        exponentially. If you are interested we have a list with the best CRM's
        on the market.
      </p>
      <a href="contact">Contact</a>
    </div>
  </div>
</div>
