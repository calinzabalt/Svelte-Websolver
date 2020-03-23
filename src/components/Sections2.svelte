<style>
  .about-section {
    width: 100%;
    background: white;
    padding: 40px 0;
    box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
    transition: 0.3s;
    max-width: 1050px;
    margin-left: auto;
    margin-right: auto;
    margin-bottom: 40px;
    margin-top: 30px;
  }
  .inner-width {
    overflow: hidden;
    padding: 0 20px;
    margin: auto;
  }
  .about-section h1 {
    text-align: center;
  }
  .border {
    width: 100px;
    height: 3px;
    background: #e74c3c;
    margin: 40px auto;
  }
  .about-section-row {
    display: flex;
    flex-wrap: wrap;
  }
  .about-section-col {
    flex: 50%;
  }
  .about {
    padding-right: 30px;
  }
  .about p {
    text-align: justify;
    margin-bottom: 20px;
  }
  .about a {
    display: inline-block;
    color: #e74c3c;
    text-decoration: none;
    border: 2px solid #e74c3c;
    border-radius: 24px;
    padding: 8px 40px;
    transition: 0.4s linear;
  }
  .about a:hover {
    color: #fff;
    background: #e74c3c;
  }

  @media screen and (max-width: 700px) {
    .about-section-col {
      flex: 100%;
      margin: 10px 0;
    }

    .about {
      text-align: center;
    }
  }
</style>

<div class="about-section">
  <div class="inner-width">
    <h1>Why To Buy From Us ?</h1>
    <div class="border" />
    <div class="about-section-row">
      <div class="about-section-col">
        <div class="about">
          <p>
            We are cheaper, faster, available 24/7 and we don't give up untill
            your website or app is up and running. If you don't believe us than
            try to reach us at this email address: websolvercalin@gmail.com or
            call us directly at this number: 40 740 691 940
          </p>
          <a href="services">Services</a>
        </div>
      </div>
    </div>
  </div>
</div>
