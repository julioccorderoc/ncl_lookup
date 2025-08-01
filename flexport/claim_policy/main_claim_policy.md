# Flexport Consolidated Claims Processing Protocol

**Document Purpose:** This protocol provides a unified, comprehensive, and sequential guide for processing all reimbursement claims with Flexport. It is designed for use by both human operators and AI systems to ensure consistent and accurate claim management.

**Primary Principle:** The claim process is divided into two main categories with different procedures: **Standard Order Claims** and **Removal Order Claims**. Identify the correct category before proceeding.

---

## **Section 1: Pre-Claim Assessment & Universal Policies**

### **1.1. Initial Claim Triage (Decision Tree)**

Use this logic to determine the correct process path:

1.  **Is the claim related to an order removing inventory from a Flexport facility (e.g., to your own warehouse, a new 3PL, or Amazon FBA)?**
    *   **Yes:** Proceed to **Section 3: Removal Order Claims**.
    *   **No:** Proceed to **Section 2: Standard Order Claims**.

2.  **Is the inquiry about a late delivery, a return-to-sender (RTS), or an order insured by a third party (e.g., Route)?**
    *   **Yes:** These are not standard claims. Refer to **Section 4: Other Inquiries & Exclusions**.

### **1.2. Universal Documentation Requirements**

The following documents may be required for any claim. Prepare them in advance.

*   **Proof of Customer Communication:** Screenshots of emails or messages from the customer detailing the issue.
    *   *Exception:* Not required for "Lost in Transit" claims.
*   **Proof of Product Issue:** Clear photos or videos showing the damage or the incorrect item received.
    *   *Applicability:* Required for "Damaged" or "Incorrect Product" claims.
*   **Proof of Cost:** Documentation to establish the value of the affected item(s). This can be:
    *   A wholesale/commercial invoice from your supplier.
    *   A retail price/customer invoice from your sales channel.
    *   **Carrier-Specific Rule:** For all claims involving **DHL and USPS** (except "Incorrect Product"), a final customer invoice is **mandatory**. It must include the customer's name, address (matching the delivery location), and the total product cost.

### **1.3. Universal Reimbursement Calculation**

Approved claims are credited to your account and applied to your next invoice. The credit value is determined as the **lesser** of the two following methods:

*   **Wholesale Cost:** Reimbursed at 100% of the value shown on the supplier/manufacturer invoice.
*   **Retail Value:** Reimbursed at **40%** of the final sale price (excluding shipping charges).

*Note: In specific cases (e.g., certain "Missing" or "Incorrect" product claims), reimbursement may be limited to fulfillment fees only.*

### **1.4. Universal Claim Restrictions**

Claims will be denied under these conditions:

*   The product is on Flexport's [restricted products list](https://support.deliverr.com/hc/en-us/articles/115002943554-Restricted-Products).
*   The damage is minor and only affects the outer shipping packaging (e.g., scuffs, creases).
*   The product was not packaged according to Flexport's [packaging requirements](https://support.portal.flexport.com/hc/en-us/articles/360056601114-Preparing-Your-Product-for-Flexport-Fulfillment-Center).
*   The order was insured by a third party (e.g., Route, OrderProtection). The claim must be filed with the insurer first.

---

## **Section 2: Standard Order Claims Process**

*   **Applies to:** Customer orders fulfilled by Flexport.
*   **Submission Method:** Flexport Seller Portal.

### **2.1. Eligibility & Timeline**

*   **Submission Window:** You have **30 calendar days** from the Promised Delivery Date (PDD) to submit a claim.
*   **Portal Availability:** The "Submit Claim" button becomes active in the Seller Portal:
    *   **3 business days** after the PDD (Standard Period).
    *   **5 business days** after the PDD (Peak Season: Nov 15 – Jan 15).

### **2.2. Claim Type Definitions & Specific Requirements**

| Claim Type | Definition / Trigger | Key Requirements & Nuances |
| :--- | :--- | :--- |
| **Lost in Transit** | No tracking updates for a set period: <br>- **Domestic:** 7 calendar days (12 in Peak Season) <br>- **International:** 21 calendar days | - No Proof of Customer Communication needed. <br>- Submit Proof of Cost. <br>- **Process:** If the "Submit Claim" button is unavailable for an international order, create a Support ticket. <br>- **Retraction Clause:** Credit may be reversed if the package is delivered within 60 days of claim approval. |
| **Delivered but Lost** | Tracking shows "Delivered," but the customer reports non-receipt after 48 hours. | - **Pre-Claim Action:** Instruct the customer to check the premises and with household members. <br>- **Required Evidence:** Proof of Customer Communication and Proof of Cost. <br>- **Nuance:** Flexport is not liable for theft post-delivery. A claim is strongest with carrier evidence of non-delivery (e.g., mail locker audit). |
| **Order Damaged** | Customer reports the product (not the box) is damaged. | - **Required Evidence:** Photos of the damaged product, Proof of Customer Communication, and Proof of Cost. <br>- **Exclusion:** Flexport is not liable for pre-existing manufacturing defects. |
| **Missing Product** | A package arrives with one or more items missing from the order. | - **Required Evidence:** Proof of Customer Communication and Proof of Cost for the missing item(s). <br>- **Reimbursement:** Varies by cause. Fulfillment errors are reimbursed for fulfillment costs only. <br>- **Exclusion:** Not available for "Parcel only" merchants. |
| **Incorrect Product** | Customer receives a product they did not order. | - **Required Evidence:** Photos of the incorrect product, Proof of Customer Communication, and Proof of Cost for the item that *should have been* sent. <br>- **Reimbursement:** Varies by cause. If the wrong item was from your inventory, reimbursement follows the standard policy. If not from your inventory, only fulfillment fees are reimbursed. <br>- **Exclusion:** Not available for "Parcel only" merchants. |

### **2.3. Post-Submission & Appeals**

*   **Tracking:** Monitor claim status (Pending, Approved, Rejected) on the Order Details page.
*   **Appeals:** A denied claim can be appealed **within 30 calendar days** of the PDD.
    *   **Appeal via Portal:** Possible for rejections due to insufficient proof of cost/communication.
    *   **Appeal via Support Team:** For all other rejection reasons, email the Support Team.

---

## **Section 3: Removal Order Claims Process**

*   **Applies to:** Orders to remove inventory from Flexport.
*   **Submission Method:** Create a Support Case in the Seller Portal.

### **3.1. Critical Warning: Shipments to FBA / Other 3PLs**

*   All removal orders sent directly to an Amazon FBA center or another 3PL are considered **"ship at own risk."**
*   By doing this, you **waive the right to file a claim** for shipments that are marked "Delivered" but cannot be located by the receiving facility.
*   Flexport is not responsible for any non-compliance fees from the receiving facility.

### **3.2. Eligibility & Timeline**

*   **Submission Window:** You have **7 calendar days** from the final delivery date to file a claim.
    *   **Peak Season (Nov 15 – Jan 15):** The window is extended to **30 calendar days**.

### **3.3. Claim Type Definitions & Specific Requirements**

| Claim Type | Definition / Trigger | Required Action & Nuances |
| :--- | :--- | :--- |
| **Short-Ships** | Fewer units are delivered than were ordered for removal. | - Create a support case for investigation. This is often an inventory count issue, not a shipping loss. |
| **No Tracking Movement** | No carrier tracking updates for 7+ calendar days. | - Create a support case. Flexport will contact the carrier. <br>- If the carrier declares the package lost, Flexport reimburses the **wholesale value**. |
| **Delivered but Lost** | Tracking shows "Delivered," but the shipment cannot be located at the destination. | - Contact Flexport support within 7 days. <br>- If Flexport provides a Proof of Delivery (POD) showing the correct address, the claim will be **denied**. |
| **Delivered Damaged** | The removed inventory arrives damaged. | - Contact Flexport support within 7 days. <br>- **Required Evidence:** A signed POD from the recipient noting the damage, and photos of the damaged products. |

---

## **Section 4: Other Inquiries & Exclusions (Not Standard Claims)**

These issues have unique processes and are **not** handled through the standard claim portal.

| Inquiry Type | Process |
| :--- | :--- |
| **Late Delivery** | Late deliveries due to carrier delays are often noted in the Seller Portal. If you believe a delay was due to a Flexport error, contact the **Support Team**. |
| **Returned to Sender (RTS) / Undeliverable** | These are handled per the [Undeliverable Orders Policy](https://support.portal.flexport.com/hc/en-us/articles/4402394009495-What-is-Flexport-s-policy-on-undeliverable-orders-and-what-do-they-mean). This is a separate process, not a claim. |
| **Third-Party Insurance** | If the customer purchased insurance (e.g., Route), the merchant must file the claim with the insurer first. Flexport reserves the right to deny claims for insured orders. |

---

## **Section 5: Glossary**

*   **PDD (Promised Delivery Date):** The estimated delivery date provided to the customer.
*   **POD (Proof of Delivery):** Confirmation from the carrier that a package was delivered, sometimes including a photo or signature.
*   **Peak Season:** November 15 to January 15. Claim windows and processing times are extended during this period.
*   **RTS (Return to Sender):** An order that is returned by the carrier because it could not be delivered.
