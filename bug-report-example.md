# 🐞 Bug Report: Cart Total Not Updating After Quantity Change

## Bug ID: AE-BUG-001 (or similar, e.g., CART-001)

## Summary
When a user modifies the quantity of an item directly within the shopping cart page, the displayed total price for the cart does not automatically reflect the updated quantity.

## Environment
* **Browser:** Chrome 125.0.6422.141 (Official Build) (64-bit)
* **Operating System:** macOS Sonoma 14.4.1 (or relevant OS)
* **Application URL:** `https://automationexercise.com/view_cart`
* **Date Found:** June 2, 2025

## Steps to Reproduce
1.  Navigate to the Home Page: `https://automationexercise.com/`
2.  Add any product to the cart with a quantity of 1 (e.g., "Blue Top").
3.  Proceed to the Cart Page (e.g., `https://automationexercise.com/view_cart`).
4.  Locate the product in the cart.
5.  Change the quantity of the product from `1` to `3` using the quantity input field directly in the cart table.
6.  Observe the "Total Amount" displayed at the bottom of the cart table.

## Expected Result
The "Total Amount" displayed on the cart page should dynamically update to `[Product Unit Price] * 3`, reflecting the new quantity.

## Actual Result
The "Total Amount" remains the same as the original quantity of 1 (i.e., `[Product Unit Price] * 1`), despite the quantity field showing `3`. The total only updates if the page is refreshed or another action is performed.

## Severity
**High** - This is a critical functional defect that directly impacts pricing accuracy and user trust, potentially leading to incorrect billing or or purchase decisions.

## Priority
**High** - Requires immediate attention as it affects core e-commerce functionality and user experience for all cart interactions.

## Reproducibility
Consistently Reproducible (100% of the time)

## Screenshots/Attachments
* [Placeholder for Screenshot 1: Cart with quantity 1 and original total]
* [Placeholder for Screenshot 2: Cart with quantity changed to 3, but incorrect total]
* [Placeholder for Video (Optional, if applicable)]

## Reported by
David Jenkins
