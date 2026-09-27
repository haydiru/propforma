# Privacy Policy — PropForma Lens

**Effective Date:** September 27, 2026  
**Last Updated:** September 27, 2026

PropForma Lens ("we," "our," or "the Extension") is committed to protecting your privacy. This Privacy Policy explains our practices regarding data collection, usage, and disclosure for our Google Chrome Extension, **PropForma: Underwriter for LoopNet & Crexi**.

---

## 1. Single Purpose & Core Functionality

PropForma Lens is designed with a single, specific purpose:  
**To extract commercial real estate listing details from LoopNet and Crexi and generate an Excel (.xlsx) financial pro forma underwriting model.**

All extraction, underwriting calculations, and Excel file generations are performed **100% locally within your client browser**.

---

## 2. Information We Do NOT Collect

We believe your investment pipeline and financial criteria are strictly confidential. Therefore:
* **No Deal or Property Data Collection:** We do not collect, transmit, store, or log any commercial property information, addresses, asking prices, financial assumptions, or underwriting results.
* **No Browsing History Collection:** We do not track, collect, or store your web browsing history outside of the active tab when you explicitly activate the extension on supported listing pages.
* **No Personal Data Selling:** We do not sell, rent, trade, or transfer any user data to third parties.
* **No Creditworthiness or Lending Evaluation:** We do not use or transfer user data to determine creditworthiness or for lending purposes.

---

## 3. Local Data Storage & Permissions

The extension requests the minimum set of permissions necessary to deliver its core functionality:

1. **`activeTab`**:
   * *Purpose:* Enables the extension popup to communicate with the currently active LoopNet or Crexi listing tab when the user clicks the extension action icon.
   * *Data Handling:* Property data read from the page DOM is held temporarily in browser memory and is never transmitted off the device.

2. **`storage`**:
   * *Purpose:* Saves user-configured default underwriting parameters (e.g., default Loan-to-Value ratio, benchmark interest rate, amortization years, vacancy allowance) and local Pro license activation status.
   * *Data Handling:* Stored locally on your device via `chrome.storage.local` / `chrome.storage.sync`.

3. **`downloads`**:
   * *Purpose:* Saves the generated `.xlsx` workbook directly to your local computer's default downloads directory when you click "Export Pro Forma (.xlsx)".

4. **Host Permissions (`*://*.loopnet.com/*`, `*://*.crexi.com/*`)**:
   * *Purpose:* Injects the content script strictly on LoopNet and Crexi listing pages to parse publicly visible property data.

---

## 4. Third-Party Services & Licensing

* **Payment & License Activation:** Payments and license keys are processed through our merchant of record, Lemon Squeezy (or Stripe). When you purchase a license or activate a Pro key, your license key is verified directly against Lemon Squeezy's secure public activation API (`https://api.lemonsqueezy.com/v1/licenses/activate`). No personal banking details, passwords, or credit card numbers are collected, handled, or stored by the PropForma Lens extension.

---

## 5. Security Architecture

Because PropForma Lens executes completely client-side in the user's browser runtime:
* Data never touches external intermediary servers.
* No remote JavaScript code is fetched, evaluated, or executed at runtime. All extension code is packaged statically within the official Chrome Web Store distribution.

---

## 6. Policy Changes & Updates

We may update this Privacy Policy from time to time. Any changes will be posted on this page with an updated "Last Updated" date.

---

## 7. Contact Information

If you have questions, feedback, or concerns regarding this Privacy Policy or your data privacy, please contact us:
* **GitHub Repository & Issues:** [https://github.com/haydiru/propforma/issues](https://github.com/haydiru/propforma/issues)
* **Website:** [https://github.com/haydiru/propforma](https://github.com/haydiru/propforma)
