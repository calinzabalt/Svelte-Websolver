<style>
  .about-section {
    width: 100%;
    background: #f1f1f1;
    padding: 40px 0;
  }
  .inner-width {
    max-width: 1000px;
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
  .skills {
    padding-left: 30px;
  }
  .skill {
    margin-bottom: 10px;
  }
  .progress {
    width: 100%;
    height: 12px;
    background: #ddd;
    border-radius: 12px;
  }
  .progress-bar {
    height: 18px;
    background: #e74c3c;
    border-radius: 12px;
  }
  .p1 {
    width: 90%;
  }
  .p2 {
    width: 100%;
  }
  .p3 {
    width: 100%;
  }
  .progress-bar span {
    float: right;
    margin-right: 6px;
    line-height: 18px;
    color: #fff;
    font-size: 12px;
  }
  @media screen and (max-width: 700px) {
    .about-section-col {
      flex: 100%;
      margin: 10px 0;
    }
    .about,
    .skills {
      padding: 0;
    }
    .about {
      text-align: center;
    }
  }
</style>

<div class="about-section">
  <div class="inner-width">
    <h1>Web Development</h1>
    <div class="border" />
    <div class="about-section-row">
      <div class="about-section-col">
        <div class="about">
          <p>
            If you need a Web Application, Presentation Website or an E-commerce
            website to sell stuff online, then we can help you. Together we can
            build fast and engaging websites that can rank very well on google
            search.
          </p>
          <a href="services">Services</a>
        </div>
      </div>
      <div class="about-section-col">
        <div class="skills">
          <div class="skill">
            <div class="title">Mobile Speed</div>
            <div class="progress">
              <div class="progress-bar p1">
                <span>90%+</span>
              </div>
            </div>
          </div>

          <div class="skill">
            <div class="title">SEO</div>
            <div class="progress">
              <div class="progress-bar p2">
                <span>100%</span>
              </div>
            </div>
          </div>

          <div class="skill">
            <div class="title">PWA</div>
            <div class="progress">
              <div class="progress-bar p3">
                <span>100%</span>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>
