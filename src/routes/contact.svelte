<script>
  let bgImage = "man.jpg";
</script>

<style>
  input[type="text"],
  textarea {
    width: 100%;
    padding: 12px;
    border: 1px solid #ccc;
    border-radius: 4px;
    box-sizing: border-box;
    margin-top: 6px;
    margin-bottom: 16px;
    resize: vertical;
  }

  input[type="submit"] {
    background-color: #4caf50;
    color: white;
    padding: 12px 20px;
    border: none;
    border-radius: 4px;
    cursor: pointer;
  }

  input[type="submit"]:hover {
    background-color: #45a049;
  }

  .container {
    border-radius: 5px;
    max-width: 800px;
    margin-left: auto;
    margin-right: auto;
    padding: 20px;
  }

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
    height: 400px;
  }

  .ptext {
    position: absolute;
    top: 50%;
    width: 100%;
    text-align: center;
    color: #000;
    font-size: 2vw;
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
  <title>Contact Us</title>
  <meta name="description" content="If you need support about websites, or other stuff related to web development, feel free to contact us. " />
</svelte:head>

<div class="pimg1" style="background-image: url('{bgImage}')">
  <div class="ptext">
    <span class="border">Do it now or regret it later</span>
  </div>
</div>

<div class="container">
  <h2>Contact Us:</h2>
  <p>
    Phone: 40 740 691 940
    <br />
    Email: websolvercalin@gmail.com
  </p>
  <form action="https://formspree.io/xdokvpao" method="POST">
    <label for="fname">Name</label>
    <input type="text" id="name" name="name" placeholder="Your name.." />

    <label for="lname">Email</label>
    <input
      type="text"
      id="email"
      name="_replyto"
      placeholder="Email address.." />

    <label for="subject">Message:</label>
    <textarea
      id="subject"
      name="subject"
      placeholder="Your message.."
      style="height:200px" />

    <input type="submit" value="Submit" />
  </form>
</div>
