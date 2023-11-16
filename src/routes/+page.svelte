<script>
    // Your Svelte script here
  </script>
  
  <style>
    body, html {
      margin: 0;
      padding: 0;
      height: 100%;
      overflow: hidden; /* Prevent scrolling */
    }
  
    .sketchfab-embed-wrapper {
      position: fixed; /* Use fixed to cover the full page */
      top: 0;
      left: 0;
      width: 100vw;
      height: 100vh;
      z-index: -1; /* Ensure it stays in the background */
    }
  
    iframe {
      width: 100%;
      height: 100%;
    }
  
    .center-container {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        position: fixed;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        z-index: 10; /* Place it above the iframe */
    }

    .title {
        font-family: 'Urbanist', sans-serif;
        font-weight: 100;
        font-size: 24px;
        color: white; /* or any color you prefer */
        margin-bottom: 20px; /* Adjust the space between the title and the button */
    }

    .apply-button {
        position: absolute;
        top: 10px;
        right: 10px;
        background-color: #92fe9d; /* Soft teal color to match the logo */
        border: none;
        border-radius: 5px;
        color: #020e27;
        padding: 10px 20px;
        font-size: 16px;
        cursor: pointer;
        transition: background-color 0.3s;
        }

    .apply-button:hover {
    background-color: #ffffff; /* Slightly darker teal on hover */
    }

    .bottom-logo {
        position: fixed;
        left: 50%;
        bottom: 10px;
        transform: translateX(-50%);
        /* Adjust width and height as needed */
        width: 150px;
        height: auto;
        z-index: 10; /* Make sure it's above other elements if needed */
    }
  </style>
  
  <div class="sketchfab-embed-wrapper">
    <iframe title="Enceladus" frameborder="0" allowfullscreen mozallowfullscreen="true" webkitallowfullscreen="true" allow="autoplay; fullscreen; xr-spatial-tracking" xr-spatial-tracking execution-while-out-of-viewport execution-while-not-rendered web-share src="https://sketchfab.com/models/65f5f87d930c4f35a4039656c266272a/embed?autospin=1&autostart=1&preload=1&ui_infos=0&ui_stop=0&ui_inspector=0&ui_watermark_link=0&ui_watermark=0&ui_hint=0&ui_ar=0&ui_help=0&ui_settings=0&ui_vr=0&ui_annotations=0"></iframe>
  </div>
  <div class="title">0L Moonshot Program</div>
  <div class="center-container">
    <div class="title">0L Moonshot Program</div>
    <button class="apply-button">Apply</button>
  </div>


  