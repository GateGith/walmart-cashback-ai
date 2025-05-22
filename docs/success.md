---
title: "Cashback Approved!"
layout: default
permalink: /success/
---

<div class="container">
  <div class="checkmark">✓</div>
  <h1>$<span id="amount">112</span> Cashback Activated!</h1>
  
  <div class="timeline">
    <div class="step completed">Offer Verified</div>
    <div class="step">Processing Payment</div>
    <div class="step">PayPal Transfer</div>
  </div>

  <div class="support">
    <p>Transaction ID: <span id="tid">WCB-${Date.now().toString().slice(-6)}</span></p>
  </div>
</div>

<script>
// Dynamic Cashback Display
const amounts = [87, 95, 112, 127];
document.getElementById('amount').textContent = 
  amounts[Math.floor(Math.random() * amounts.length)];

// Block repeat visits
document.cookie = "cashback_claimed=1; max-age=2592000; path=/";
</script>
