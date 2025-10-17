<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>UI Universe Card (Website Style)</title>
  <style>
    /* From Uiverse.io by Smit-Prajapati | Modified for full website look */
    body {
      background: #111827;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
      font-family: "Poppins", Arial, sans-serif;
    }

    .card {
      width: 90%;
      max-width: 800px;
      border-radius: 25px;
      background: #1b233d;
      padding: 20px;
      overflow: hidden;
      box-shadow: rgba(100, 100, 111, 0.25) 0px 10px 30px 0px;
      transition: transform 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    }

    .card:hover {
      transform: scale(1.02);
    }

    .card .top-section {
      height: 250px;
      border-radius: 20px;
      display: flex;
      flex-direction: column;
      background: linear-gradient(45deg, rgb(4, 159, 187) 0%, rgb(80, 246, 255) 100%);
      position: relative;
    }

    .card .top-section .border {
      border-bottom-right-radius: 15px;
      height: 50px;
      width: 250px;
      background: #1b233d;
      position: relative;
      transform: skew(-40deg);
      box-shadow: -15px -15px 0 0 #1b233d;
    }

    .card .top-section .border::before {
      content: "";
      position: absolute;
      width: 25px;
      height: 25px;
      top: 0;
      right: -25px;
      border-top-left-radius: 15px;
      box-shadow: -8px -8px 0 2px #1b233d;
    }

    .card .top-section::before {
      content: "";
      position: absolute;
      top: 50px;
      left: 0;
      height: 25px;
      width: 25px;
      border-top-left-radius: 20px;
      box-shadow: -8px -8px 0 2px #1b233d;
    }

    .card .top-section .icons {
      position: absolute;
      top: 0;
      width: 100%;
      height: 60px;
      display: flex;
      justify-content: space-between;
    }

    .card .top-section .icons .logo {
      height: 100%;
      padding: 10px 0 10px 25px;
    }

    .card .top-section .icons .social-media {
      height: 100%;
      padding: 12px 25px;
      display: flex;
      gap: 15px;
    }

    .card .top-section .icons .social-media .svg {
      height: 100%;
      fill: #1b233d;
      cursor: pointer;
      transition: fill 0.3s ease;
    }

    .card .top-section .icons .social-media .svg:hover {
      fill: white;
    }

    .card .bottom-section {
      margin-top: 25px;
      padding: 20px 10px;
    }

    .card .bottom-section .title {
      display: block;
      font-size: 32px;
      font-weight: 700;
      color: white;
      text-align: center;
      letter-spacing: 3px;
    }

    .card .bottom-section .row {
      display: flex;
      justify-content: space-between;
      margin-top: 30px;
      flex-wrap: wrap;
    }

    .card .bottom-section .row .item {
      flex: 1;
      text-align: center;
      padding: 10px;
      color: rgba(170, 222, 243, 0.9);
      min-width: 150px;
    }

    .card .bottom-section .row .item .big-text {
      font-size: 24px;
      display: block;
      font-weight: 600;
    }

    .card .bottom-section .row .item .regular-text {
      font-size: 14px;
    }

    .card .bottom-section .row .item:nth-child(2) {
      border-left: 1px solid rgba(255, 255, 255, 0.15);
      border-right: 1px solid rgba(255, 255, 255, 0.15);
    }

    @media (max-width: 600px) {
      .card {
        width: 95%;
      }

      .card .top-section {
        height: 200px;
      }

      .card .bottom-section .title {
        font-size: 24px;
      }

      .card .bottom-section .row {
        flex-direction: column;
        align-items: center;
        gap: 10px;
      }

      .card .bottom-section .row .item:nth-child(2) {
        border: none;
      }
    }
  </style>
</head>
<body>
  <div class="card">
    <div class="top-section">
      <div class="border"></div>
      <div class="icons">
        <div class="logo">
          <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 94 94" class="svg">
            <path fill="white" d="M38.0481 4.82927C38.0481 2.16214 40.018 0 42.4481 0H51.2391C53.6692 0 55.6391 2.16214 55.6391 4.82927V40.1401C55.6391 48.8912 53.2343 55.6657 48.4248 60.4636C43.6153 65.2277 36.7304 67.6098 27.7701 67.6098C18.8099 67.6098 11.925 65.2953 7.11548 60.6663C2.37183 56.0036 3.8147e-06 49.2967 3.8147e-06 40.5456V4.82927C3.8147e-06 2.16213 1.96995 0 4.4 0H13.2405C15.6705 0 17.6405 2.16214 17.6405 4.82927V39.1265C17.6405 43.7892 18.4805 47.2018 20.1605 49.3642C21.8735 51.5267 24.4759 52.6079 27.9678 52.6079C31.4596 52.6079 34.0127 51.5436 35.6268 49.4149C37.241 47.2863 38.0481 43.8399 38.0481 39.0758V4.82927Z"></path>
            <path fill="white" d="M86.9 61.8682C86.9 64.5353 84.9301 66.6975 82.5 66.6975H73.6595C71.2295 66.6975 69.2595 64.5353 69.2595 61.8682V4.82927C69.2595 2.16214 71.2295 0 73.6595 0H82.5C84.9301 0 86.9 2.16214 86.9 4.82927V61.8682Z"></path>
            <path fill="white" d="M2.86102e-06 83.2195C2.86102e-06 80.5524 1.96995 78.3902 4.4 78.3902H83.6C86.0301 78.3902 88 80.5524 88 83.2195V89.1707C88 91.8379 86.0301 94 83.6 94H4.4C1.96995 94 0 91.8379 0 89.1707L2.86102e-06 83.2195Z"></path>
          </svg>
        </div>
        <div class="social-media">
          <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 30 30" class="svg">
            <path d="M 9.9980469 3 C 6.1390469 3 3 6.1419531 3 10.001953 L 3 20.001953 C 3 23.860953 6.1419531 27 10.001953 27 L 20.001953 27 C 23.860953 27 27 23.858047 27 19.998047 L 27 9.9980469 C 27 6.1390469 23.858047 3 19.998047 3 L 9.9980469 3 z M 22 7 C 22.552 7 23 7.448 23 8 C 23 8.552 22.552 9 22 9 C 21.448 9 21 8.552 21 8 C 21 7.448 21.448 7 22 7 z M 15 9 C 18.309 9 21 11.691 21 15 C 21 18.309 18.309 21 15 21 C 11.691 21 9 18.309 9 15 C 9 11.691 11.691 9 15 9 z M 15 11 A 4 4 0 0 0 11 15 A 4 4 0 0 0 15 19 A 4 4 0 0 0 19 15 A 4 4 0 0 0 15 11 z"></path>
          </svg>
          <svg class="svg" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512">
            <path d="M459.37 151.716c..."></path>
          </svg>
          <svg class="svg" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 640 512">
            <path d="M524.531,69.836a1.5,1.5..."></path>
          </svg>
        </div>
      </div>
    </div>
    <div class="bottom-section">
      <span class="title">UNIVERSE OF UI</span>
      <div class="row row1">
        <div class="item">
          <span class="big-text">2,626</span>
          <span class="regular-text">UI Elements</span>
        </div>
        <div class="item">
          <span class="big-text">100%</span>
          <span class="regular-text">Free for Use</span>
        </div>
        <div class="item">
          <span class="big-text">38,631</span>
          <span class="regular-text">Contributors</span>
        </div>
      </div>
    </div>
  </div>
</body>
</html>
