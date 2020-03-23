<script>

</script>

<style>
  footer {
    background: #f1f1f1;
    padding: 90px 0;
  }

  .footer-container {
    max-width: 1300px;
    margin: auto;
    padding: 0 20px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap-reverse;
  }

  .social-media {
    margin: 20px 0;
  }

  .social-media a {
    color: #001a21;
    margin-right: 25px;
    font-size: 22px;
    text-decoration: none;
    transition: 0.3s linear;
  }

  .social-media a:hover {
    color: #fc5c65;
  }

  .right-col h1 {
    font-size: 26px;
  }

  .newsletter-form {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
  }

  .txtb {
    flex: 1;
    padding: 18px 40px;
    font-size: 16px;
    color: #293043;
    background: #ddd;
    border: none;
    font-weight: 700;
    outline: none;
    border-radius: 30px;
    min-width: 260px;
  }

  .btn {
    padding: 18px 40px;
    font-size: 16px;
    color: #f1f1f1;
    background: #fc5c65;
    border: none;
    font-weight: 700;
    outline: none;
    border-radius: 30px;
    margin-left: 20px;
    cursor: pointer;
    transition: opacity 0.3s linear;
  }

  .btn:hover {
    opacity: 0.7;
  }

  @media screen and (max-width: 960px) {
    .footer-container {
      max-width: 600px;
    }
    .right-col {
      width: 100%;
      margin-bottom: 60px;
    }

    .left-col {
      width: 100%;
      text-align: center;
    }
  }

  @media screen and (max-width: 700px) {
    .btn {
      margin: 0;
      width: 100%;
      margin-top: 20px;
    }
  }

  p {
    font-size: 18px;
  }

  .right-col a {
    display: inline-block;
    color: #e74c3c;
    text-decoration: none;
    border: 2px solid #e74c3c;
    border-radius: 24px;
    padding: 3px 20px;
    transition: 0.4s linear;
    margin-bottom: 5px;
  }

  .right-col a:hover {
    color: #fff;
    background: #e74c3c;
  }
</style>

<footer>
  <div class="footer-container">
    <div class="left-col">
      <h1>Social Media</h1>
      <div class="social-media">

        <a
          target="blank"
          href="https://www.linkedin.com/in/cozma-viorel-calin-947658145/detail/recent-activity/">
          <img alt="linkedin" src="linkedin.svg" height="30" />
        </a>

        <a target="blank" href="https://www.facebook.com/CozmaViorelCalinPFA/">
          <img alt="facebook" src="facebook.svg" height="30" />
        </a>

        <a target="blank" href="https://twitter.com/Cozmaviorelcal1">
          <img alt="twitter" src="twitter.svg" height="30" />
        </a>
        <a target="blank" href="https://www.instagram.com/cozmaviorelcalin/">
          <img alt="instagram" src="instagram.svg" height="30" />
        </a>
        <a
          target="blank"
          href="https://www.youtube.com/channel/UC2CNVDGd1odpr7UqsiIM68g?view_as=subscriber">
          <img alt="youtube" src="youtube.svg" height="30" />
        </a>

      </div>
      <p>
        Phone: 40 740 691 940
        <br />
        Email: websolvercalin@gmail.com
      </p>
      <p class="rights-text">
        © 2020 Created By Websolver All Rights Reserved.
      </p>
    </div>

    <div class="right-col">
      <h1>Useful Links:</h1>
      <a href="terms">Privacy policy</a>
      <br />
      <a href="terms">Terms and conditions</a>
      <p>Enter Your Email to get our news and updates.</p>
      <form action="" class="newsletter-form">
        <input type="text" class="txtb" placeholder="Work in Progress" />
        <input type="submit" disabled class="btn" value="submit" />
      </form>
    </div>
  </div>
</footer>
