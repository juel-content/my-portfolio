# How Mobile Payments Work: NFC + Tokenization

When you tap your phone to pay, your real card number is **not** sent.  
Instead, a **token** (a safe stand-in number) is used.

---

## Step 1 — Your phone stores a token
- Your bank/card network creates a token that represents your real card.  
- The token lives in a secure part of your device (called the “secure element”).  

---

## Step 2 — Tap with NFC
- NFC allows your phone and the payment terminal to communicate at close range.  
- Your phone sends the **token** + a one-time cryptogram (like a digital fingerprint).  

---

## Step 3 — Authorization
- The terminal sends the token to the payment network.  
- The network swaps the token for your real card **behind the scenes** and asks your bank:  
  “Approve this purchase?”  

---

## Step 4 — Response
- Bank approves or declines.  
- The result flows back through the payment network to the merchant.  
- You see **Approved** on your phone or the terminal.  

---

## Why tokenization matters
- Merchants never see or store your real card number.  
- If a hacker steals the token, it’s useless outside that specific device.  
- This greatly reduces fraud risk.  

---

## Summary
Mobile payments combine:
- **NFC** for fast, wireless communication  
- **Tokenization** for safety  
- **Cryptograms** for transaction security  

Result: payments that are quick, secure, and private.  
