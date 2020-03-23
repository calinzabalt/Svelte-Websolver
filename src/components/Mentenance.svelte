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
    width: 300px;
    height: 100%;
    display: inline-block;
    margin: 20px;
  }

  .card:hover {
    box-shadow: 0 8px 16px 0 rgba(0, 0, 0, 0.2);
  }

  .container {
    padding: 2px 16px;
    text-align: left;
  }
</style>

<div class="card-container">
  <div class="card">
    <div class="container">
      <p>
        <strong>
          Maintenance
          <br />
          20€/month
        </strong>
      </p>
      <p>
        - Bug fixes
        <br />
        - Add Content
        <br />
        - Technical Testing
      </p>

    </div>
  </div>
  <div class="card">
    <div class="container">
      <p>
        <strong>
          Maintenance
          <br />
          41€/month
        </strong>
      </p>
      <p>
        - Bug fixes
        <br />
        - Add Content
        <br />
        - Website structure
        <br />
        - Technical Testing
        <br />
        - SEO optimization
      </p>
    </div>
  </div>
  <div class="card">
    <div class="container">
      <p>
        <strong>
          Maintenance
          <br />
          104€/month
        </strong>
      </p>
      <p>
        - Bug fixes
        <br />
        - Add Content
        <br />
        - Website structure
        <br />
        - SEO optimization
        <br />
        - Website Purpose
        <br />
        - Objectives
        <br />
        - Target Audience
        <br />
        - Technical Testing
      </p>
    </div>
  </div>
</div>
