
<link rel="apple-touch-icon" sizes="180x180" href="/portfolio/apple-touch-icon.png">
<link rel="icon" type="image/png" sizes="32x32" href="/portfolio/favicon-32x32.png">
<link rel="icon" type="image/png" sizes="16x16" href="/portfolio/favicon-16x16.png">
<link rel="manifest" href="/portfolio/site.webmanifest">
<link rel="mask-icon" href="/portfolio/safari-pinned-tab.svg" color="#5bbad5">
<link rel="shortcut icon" href="/portfolio/favicon.ico">
<meta name="msapplication-TileColor" content="#da532c">
<meta name="msapplication-config" content="/portfolio/browserconfig.xml">
<meta name="theme-color" content="#ffffff">

<script>
    
// This is the "Offline page" service worker

// Add this below content to your HTML page, or add the js file to your page at the very top to register service worker

// Check compatibility for the browser we're running this in
if ("serviceWorker" in navigator) {
  if (navigator.serviceWorker.controller) {
    console.log("[PWA Builder] active service worker found, no need to register");
  } else {
    // Register the service worker
    navigator.serviceWorker
      .register("pwabuilder-sw.js", {
        scope: "./"
      })
      .then(function (reg) {
        console.log("[PWA Builder] Service worker has been registered for scope: " + reg.scope);
      });
  }
}
</script>

# Protfolio

## Nigel Morris

[Facebook](https://www.facebook.com)
