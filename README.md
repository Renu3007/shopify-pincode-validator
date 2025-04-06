# Shopify Pincode Validator

This project adds a Pincode Delivery Validator to the Shopify product page using a custom Liquid section and Google Sheets.

## Features

- Input field for users to enter a pincode
- Validates against a list of serviceable pincodes stored in Google Sheets
- Real-time response (delivery available or not)
- Simple and clean UI with responsive design
- Lightweight and doesn’t require external apps

## Tech Stack

- Shopify Liquid
- Google Apps Script (for backend)
- Google Sheets (for pincode data)
- HTML, CSS, JavaScript

## Live Google Apps Script URL

https://script.google.com/macros/s/AKfycbzxblaYpS43Xzkb4EJJRExFlJhg1aCEHl7GEtJYdzkeNnd_5h1zX4K29T0eDNLAd5kXHg/exec

## Coding Approach

1. Created a new Liquid section named `pincode-validator.liquid` in the theme.
2. Added an input field and a button that captures user pincode.
3. Used JavaScript `fetch()` to get data from a public Google Sheet via Apps Script.
4. Parsed the response and matched the entered pincode with the available list.
5. Displayed appropriate messages:
   - "Delivery available in your area"
   - "Sorry, delivery not available in your area"
6. Styled the section using custom CSS for responsive design.

## Files Involved

- `sections/pincode-validator.liquid` — main logic and design
- Google Apps Script connected to Google Sheet
- README.md — this file

## How to Use

1. Add `pincode-validator.liquid` to your theme's `sections/` folder.
2. Add the section to the product page using `product.json` or the theme editor.
3. Make sure the section uses your deployed Google Apps Script URL.
4. Save, test, and publish your theme.
