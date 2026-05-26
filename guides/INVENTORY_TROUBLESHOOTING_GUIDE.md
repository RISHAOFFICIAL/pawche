# Pawché — Inventory Troubleshooting Guide

This guide addresses common inventory and stock-related questions for the Pawché luxury storefront, specifically for the dropshipping model used with DSers or AutoDS.

## 1. Why do my products show "100" in stock?
To ensure your store is launch-ready, we have pre-set the inventory level for all **87 products** to **100 units** in the master CSV. 
- **Reason**: This prevents products from appearing as "Sold Out" immediately after import.
- **Next Step**: Once you connect your store to **DSers** or **AutoDS**, these apps will begin syncing the *actual* stock levels from the AliExpress suppliers.

## 2. Products showing as "Sold Out" (Zero Stock Issue)
If a product shows as "Sold Out" on your storefront, check the following in your Shopify Admin:

### **Check A: "Continue selling when out of stock"**
For dropshipping, this is the most critical setting.
1. Go to **Products** in Shopify.
2. Click on the product and scroll to the **Variants** section.
3. Ensure the checkbox **"Continue selling when out of stock"** is **checked**.
4. *Why?*: AliExpress stock fluctuates. This setting ensures you never miss a sale even if the supplier's stock temporarily hits zero.

### **Check B: Inventory Management**
1. Ensure the **"Track quantity"** setting is enabled.
2. Ensure **"Inventory managed by"** is set to **Shopify** (unless specifically using an app that requires otherwise).

---

## 3. Syncing with DSers / AutoDS
If you notice stock levels dropping to 0 automatically, your fulfillment app is syncing with the supplier.

### **If an item is truly out of stock at the supplier:**
1. **DSers**: Navigate to the **Open Orders** or **My Products** tab in DSers. It will flag products that are "Out of Stock" or "No longer available."
2. **Action**: You can either:
   - Find an alternative supplier in AliExpress for the same product and map it.
   - Temporarily unpublish the product in Shopify until it's restocked.

### **To override sync and show stock:**
If you want to force an item to show as available regardless of sync:
1. In **DSers Settings**, look for **Inventory Sync**.
2. You can disable sync for specific products or set a "Fixed Quantity" (e.g., always show 10 units).

---

## 4. Bulk Updating Inventory
If you need to reset all products to "100" or enable "Continue Selling" for everything:
1. Go to **Products**.
2. Select all products using the checkbox at the top.
3. Click **Bulk Edit**.
4. Add the columns: **"Track quantity"**, **"Continue selling when out of stock"**, and **"Stock"**.
5. Update all rows and click **Save**.

---

## 5. Troubleshooting "Unavailable" at Checkout
If a product has stock but shows as "Unavailable" or "This item can't be shipped" at checkout:
- **Shipping Profile**: Ensure the product is assigned to a **Shipping Profile** (Settings > Shipping and Delivery).
- **Origin**: Verify your shipping origin is set to **Detroit, Michigan** as per brand guidelines.

---

*For luxury concierge assistance with inventory mapping, contact your technical operator.*
