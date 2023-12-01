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
  
/* Container for the top area */
.top-container {
  position: relative;
  width: 100%;
  height: 60px; /* Adjust the height as needed to contain the title and button */
}

.title {
  position: absolute;
  top: 50%;
  left: 10px;
  transform: translateY(-50%);
  font-family: 'Urbanist', sans-serif;
  font-weight: 100;
  font-size: 24px;
  color: white; /* or any color you prefer */
}

.apply-button {
  position: absolute;
  top: 50%;
  right: 10px;
  transform: translateY(-50%);
  background-color: #4DB6AC; /* Soft teal color to match the logo */
  border: none;
  border-radius: 5px;
  color: white;
  padding: 10px 20px;
  font-size: 16px;
  cursor: pointer;
  transition: background-color 0.3s;
}

.apply-button:hover {
  background-color: #009688; /* Slightly darker teal on hover */
}


    .bottom-logo {
        position: fixed;
        left: 50%;
        bottom: 10px;
        transform: translateX(-50%);
        /* Adjust width and height as needed */
        width: 100px;
        height: auto;
        z-index: 10; /* Make sure it's above other elements if needed */
        transition: transform 0.3s ease; /* Ensure smooth transition */
        transform-origin: center; /* Set the origin of transformation */
    }

.bottom-logo:hover {
  transform: translateX(-50%) scale(1.2); /* Scale and keep centered */
}
  </style>
  
  <div class="sketchfab-embed-wrapper">
    <iframe title="Enceladus" frameborder="0" allowfullscreen mozallowfullscreen="true" webkitallowfullscreen="true" allow="autoplay; fullscreen; xr-spatial-tracking" xr-spatial-tracking execution-while-out-of-viewport execution-while-not-rendered web-share src="https://sketchfab.com/models/65f5f87d930c4f35a4039656c266272a/embed?autospin=1&autostart=1&preload=1&ui_infos=0&ui_stop=0&ui_inspector=0&ui_watermark_link=0&ui_watermark=0&ui_hint=0&ui_ar=0&ui_help=0&ui_settings=0&ui_vr=0&ui_annotations=0"></iframe>
  </div>
  <div class="top-container">
    <div class="title">0L Moonshot Program</div>
    <a href="https://apply.enceladus.life"><button class="apply-button"  >Apply</button></a>
  </div>
  <a href="https://github.com/enceladus-labs" target="_blank">
    <img src="logo.svg" alt="Enceladus Labs Inc Logo" class="bottom-logo">
</a>

  