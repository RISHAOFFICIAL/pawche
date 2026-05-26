# Pawché — Official Brand Email Setup Guide

To maintain the luxury brand identity and ensure seamless customer communication, the following official email addresses must be activated for the `pawche.store` domain.

## 📧 Required Email Addresses
1. **support@pawche.store** — Primary customer concierge and order updates.
2. **privacy@pawche.store** — GDPR, CCPA, and privacy-related inquiries (referenced in Privacy Policy).
3. **legal@pawche.store** — Terms of service and official legal notices (referenced in Terms of Service).

---

## 🛠 Step 1: Mailbox Creation
Since these are custom domain emails, you must create them through your domain registrar (e.g., Namecheap, GoDaddy) or your email hosting provider (e.g., Google Workspace, Microsoft 365, Zoho Mail).

### **Option A: Google Workspace (Recommended)**
1. Log in to your **Google Admin Console**.
2. Navigate to **Users** > **Add new user**.
3. Create a primary user (e.g., `admin@pawche.store`).
4. Add **Aliases** for `support`, `privacy`, and `legal` so they all land in one inbox, OR create separate users if you have a team.

### **Option B: Shopify Email Forwarding (Basic)**
If your domain is managed by Shopify:
1. Go to **Settings** > **Domains**.
2. Click your domain name.
3. In the **Email Forwarding** section, click **Add forwarding email**.
4. Map `support@pawche.store` to your personal email address. Repeat for `privacy` and `legal`.

---

## 🔗 Step 2: Shopify Integration
Once the addresses are active, update your Shopify settings:
1. **Sender Email**: Go to **Settings** > **Notifications** > **Sender email**. Set this to `support@pawche.store`.
2. **Store Email**: Go to **Settings** > **General** > **Store details**. Set the "Account email" to `support@pawche.store`.

---

## ✉️ Step 3: Klaviyo & Marketing Integration
If you are using Klaviyo for the staged email flows:
1. Log in to **Klaviyo**.
2. Go to **Settings** > **Organization** > **Email Settings**.
3. Set the **Default From Email** to `support@pawche.store`.
4. Set the **Default From Name** to `Pawché Concierge`.

---

## ✅ Integration Check
The following staged documents already reference these email addresses:
- **Privacy Policy**: `privacy@pawche.store`
- **Terms of Service**: `legal@pawche.store`
- **Refund Policy**: `support@pawche.store`
- **Shipping Policy**: `support@pawche.store`

**Note**: Ensure you verify these email addresses in Shopify and Klaviyo by clicking the verification links sent to the new inboxes.
