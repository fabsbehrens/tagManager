// Einbindung vom Tagmanager (Consent Mode 2 in Contao)

// Data Layer Defaults einstellen
<script data-cookieconsent="ignore">
  console.log('setting data layer to default');
  window.dataLayer = window.dataLayer || [];
  function gtag() {
    dataLayer.push(arguments);
  }
  gtag("consent", "default", {
    ad_personalization: "denied",
    ad_storage: "denied",
    ad_user_data: "denied",
    analytics_storage: "denied",
    functionality_storage: "denied",
    personalization_storage: "denied",
    security_storage: "granted",
    wait_for_update: 500,
  });
  gtag("set", "ads_data_redaction", true);
  gtag("set", "url_passthrough", true);
</script>

// User Centrics laden
<script id="usercentrics-cmp" async data-eu-mode="true" data-settings-id="5iW4gHTe2" src="https://app.eu.usercentrics.eu/browser-ui/latest/loader.js"></script>

// Tagmanager Einbindung
<!-- Google Tag Manager -->
<script type="text/plain" data-usercentrics="Google Tag Manager">
  (function(w,d,s,l,i){
    w[l]=w[l]||[];
    w[l].push({'gtm.start': new Date().getTime(),event:'gtm.js'});
    var f=d.getElementsByTagName(s)[0],
        j=d.createElement(s),dl=l!='dataLayer'?'&l='+l:'';j.async=true;j.src=
        'https://www.googletagmanager.com/gtm.js?id='+i+dl;f.parentNode.insertBefore(j,f);
  })(window,document,'script','dataLayer','GTM-PPZQB8NB');
</script>

<script type="application/javascript" src="https://privacy-proxy.usercentrics.eu/latest/uc-block.bundle.js"></script>

