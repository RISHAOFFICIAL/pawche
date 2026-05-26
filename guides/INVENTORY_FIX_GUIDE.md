# Pawché — Inventory & "Zero Stock" Fix Guide

If your imported products show **0 in stock** despite the CSV specifying 100, follow these steps to restore your luxury inventory levels.

## 🔍 Why is this happening?
The most common reason for "Zero Stock" after a CSV import is **Multiple Locations**. 
Shopify's standard Product CSV (which we used) can only import inventory quantities for stores with a **single location**. If your store has multiple locations (e.g., a default location + an app-specific location like DSers), Shopify ignores the "Variant Inventory Qty" column to prevent stock from being assigned to the wrong place.

---

## 🛠 Fix 1: The Bulk Edit Method (Fastest)
This is the easiest way to reset all 87 products to "In Stock" (100 units) and ensure they are sellable.

1.  Log in to your **Shopify Admin**.
2.  Go to **Products**.
3.  Click the checkbox at the top to **Select all** products (Ensure you click "Select all 87 products in this store" if prompted).
4.  Click **Bulk Edit**.
5.  Click **Columns** (top right) and ensure the following are checked:
    *   **Stock** (Select your primary location, e.g., "Detroit" or "Main").
    *   **Continue selling when out of stock**.
    *   **Inventory managed by**.
6.  **Update the values**:
    *   Set **Inventory managed by** to `Shopify`.
    *   Set **Stock** to `100` for the first row, then drag the small square down to fill all rows.
    *   Ensure **Continue selling when out of stock** is checked for all.
7.  Click **Save**.

---

## 🛠 Fix 2: The "Inventory CSV" Method (Advanced)
If you have many locations and want to be precise:

1.  Go to **Products** > **Inventory**.
2.  Click **Export** to get a template of your current inventory (this includes a `Location` column).
3.  Open the exported file and set the `Available` column to `100` for your primary location.
4.  Click **Import** on the Inventory page and upload the modified file.

---

## 🛠 Fix 3: DSers Sync
Once you connect **DSers**, the app will take over inventory management. 

1.  Open the **DSers App**.
2.  Go to **Setting** > **Inventory**.
3.  Ensure **Inventory Sync** is enabled.
4.  *Note*: DSers will eventually overwrite your "100" with the *actual* stock from the AliExpress supplier. This is desired for accuracy!

---

## ✅ Final Verification
Check a product on your storefront. If the "Add to Cart" button is visible, the fix is successful. If it still says "Sold Out," double-check that the **Variant Inventory Policy** is set to `Continue` (Allow overselling).

*For additional technical support, contact the Pawché Store Ops team.*
