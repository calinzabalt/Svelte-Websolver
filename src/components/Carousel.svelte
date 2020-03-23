<style>
  #slider {
    margin: 0 auto;
    width: 800px;
    max-width: 100%;
    text-align: center;
  }
  #slider input[type="radio"] {
    display: none;
  }
  #slider label {
    cursor: pointer;
    text-decoration: none;
  }
  #slides {
    padding: 10px;
    border: 3px solid #ccc;
    background: #fff;
    position: relative;
    z-index: 1;
  }
  #overflow {
    width: 100%;
    overflow: hidden;
  }
  #slide1:checked ~ #slides .inner {
    margin-left: 0;
  }
  #slide2:checked ~ #slides .inner {
    margin-left: -100%;
  }
  #slide3:checked ~ #slides .inner {
    margin-left: -200%;
  }
  #slide4:checked ~ #slides .inner {
    margin-left: -300%;
  }
  #slides .inner {
    transition: margin-left 800ms cubic-bezier(0.77, 0, 0.175, 1);
    width: 400%;
    line-height: 0;
    height: 300px;
  }
  #slides .slide {
    width: 25%;
    float: left;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100%;
    color: #fff;
  }
  #slides .slide_1 {
    background-image: url("https://drive.google.com/uc?id=1HKlxMZXs1-5JgqvPRdQv5dpG_SjaXXi4");
    background-image: -webkit-image-set(
      url("https://drive.google.com/uc?id=1F-3Wjcb5vwDWCUcFpURaJgm_AeimdkC_") 1x
    );
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
  }
  #slides .slide_2 {
    background-image: url("https://drive.google.com/uc?id=1qFKXA77HPMySSle1xb3wF5QO2s5CMKmJ");
    background-image: -webkit-image-set(
      url("https://drive.google.com/uc?id=1HV25Z1xwRKG8qhHdO6KGHylKHASFu_TD") 1x
    );
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
  }
  #slides .slide_3 {
    background-image: url("https://drive.google.com/uc?id=1sXv1u94J8YjIE1anLWDeOhtIUqwO5nmO");
    background-image: -webkit-image-set(
      url("https://drive.google.com/uc?id=1gfpidpavCE_qTqi1yGmMxUJr2gBLABN0") 1x
    );
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
  }
  #slides .slide_4 {
    background-image: url("https://drive.google.com/uc?id=1DAry8cItCp39XcskBRLYldzsUEBH2Y1w");
    background-image: -webkit-image-set(
      url("https://drive.google.com/uc?id=1euP1uJc6nXD-9bhToQ3fyTMSP-t6_ZyK") 1x
    );
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
  }
  #controls {
    margin: -180px 0 0 0;
    width: 100%;
    height: 50px;
    z-index: 3;
    position: relative;
  }
  #controls label {
    transition: opacity 0.2s ease-out;
    display: none;
    width: 50px;
    height: 50px;
    opacity: 0.4;
  }
  #controls label:hover {
    opacity: 1;
  }
  #slide1:checked ~ #controls label:nth-child(2),
  #slide2:checked ~ #controls label:nth-child(3),
  #slide3:checked ~ #controls label:nth-child(4),
  #slide4:checked ~ #controls label:nth-child(1) {
    background: url(https://image.flaticon.com/icons/svg/130/130884.svg)
      no-repeat;
    float: right;
    margin: 0 -50px 0 0;
    display: block;
  }
  #slide1:checked ~ #controls label:nth-last-child(2),
  #slide2:checked ~ #controls label:nth-last-child(3),
  #slide3:checked ~ #controls label:nth-last-child(4),
  #slide4:checked ~ #controls label:nth-last-child(1) {
    background: url(https://image.flaticon.com/icons/svg/130/130882.svg)
      no-repeat;
    float: left;
    margin: 0 0 0 -50px;
    display: block;
  }
  #bullets {
    margin: 150px 0 0;
    text-align: center;
  }
  #bullets label {
    display: inline-block;
    width: 10px;
    height: 10px;
    border-radius: 100%;
    background: #ccc;
    margin: 0 10px;
  }
  #slide1:checked ~ #bullets label:nth-child(1),
  #slide2:checked ~ #bullets label:nth-child(2),
  #slide3:checked ~ #bullets label:nth-child(3),
  #slide4:checked ~ #bullets label:nth-child(4) {
    background: #444;
  }
  @media screen and (max-width: 900px) {
    #slide1:checked ~ #controls label:nth-child(2),
    #slide2:checked ~ #controls label:nth-child(3),
    #slide3:checked ~ #controls label:nth-child(4),
    #slide4:checked ~ #controls label:nth-child(1),
    #slide1:checked ~ #controls label:nth-last-child(2),
    #slide2:checked ~ #controls label:nth-last-child(3),
    #slide3:checked ~ #controls label:nth-last-child(4),
    #slide4:checked ~ #controls label:nth-last-child(1) {
      margin: 0;
    }
    #slides {
      max-width: calc(100% - 140px);
      margin: 0 auto;
    }
  }
</style>

<div id="slider">
  <input type="radio" name="slider" id="slide1" checked />
  <input type="radio" name="slider" id="slide2" />
  <input type="radio" name="slider" id="slide3" />
  <input type="radio" name="slider" id="slide4" />
  <div id="slides">
    <div id="overflow">
      <div class="inner">
        <div class="slide slide_1">
          <div class="slide-content" />
        </div>
        <div class="slide slide_2">
          <div class="slide-content" />
        </div>
        <div class="slide slide_3">
          <div class="slide-content" />
        </div>
        <div class="slide slide_4">
          <div class="slide-content" />
        </div>
      </div>
    </div>
  </div>
  <div id="controls">
    <label for="slide1" />
    <label for="slide2" />
    <label for="slide3" />
    <label for="slide4" />
  </div>
  <div id="bullets">
    <label for="slide1" />
    <label for="slide2" />
    <label for="slide3" />
    <label for="slide4" />
  </div>
</div>
