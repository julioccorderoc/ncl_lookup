# Shopify Consolidated Chargeback & Inquiry Protocol

**Document Purpose:** This protocol provides a unified, sequential guide for managing all Shopify payment disputes. It is designed to be the single source of truth for human agents and AI systems to ensure consistent, accurate, and strategic handling of chargebacks and inquiries.

## **Section 1: Core Concepts & Triage**

This section defines the fundamental concepts and the initial decision-making process.

### **1.1. Key Definitions**

*   **Inquiry:** A preliminary step initiated by a cardholder's bank to question a charge. **No funds are withdrawn from you during an inquiry.** It is a request for information that may escalate to a chargeback if unresolved.
*   **Chargeback:** A formal dispute where the cardholder's bank **immediately reverses the charge**, withdrawing the disputed amount plus a separate **chargeback fee** from your account.
*   **Cardholder:** The customer or individual who owns the credit card used for the transaction.
*   **Issuing Bank:** The cardholder's bank, which makes the final decision on the dispute.

### **1.2. Shopify's Role (Critical Principle)**

*   Shopify acts as a **conduit**, not a judge. They provide the platform to submit evidence but are not involved in the decision-making process.
*   The **issuing bank** has the final authority to resolve the dispute.
*   Shopify is **not liable** for chargebacks and does not cover funds reversed by banks.

### **1.3. Initial Triage: Is it a Chargeback or an Inquiry?**

This is the first and most important step to determine the correct procedure.

1.  **Have funds been immediately deducted from your account along with a fee?**
    *   **Yes:** It is a **Chargeback**. Proceed to **Section 2.1**.
    *   **No:** It is an **Inquiry**. Proceed to **Section 2.2**.

---

## **Section 2: The Dispute Process Flow**

### **2.1. Chargeback Process Flow**

1.  **Initiation:** The cardholder disputes a charge with their bank.
2.  **Funds Withdrawal:** The issuing bank immediately debits the disputed amount and a chargeback fee from your Shopify Payouts account.
3.  **Evidence Request:** The credit card company requests evidence from you via your Shopify Admin.
4.  **Response Window:** You have a limited time (typically 7-21 days) to submit a response.
5.  **Evidence Submission:** You submit all relevant evidence through the Shopify Admin portal.
6.  **Review:** The credit card company reviews the evidence. This can take up to **75 days** after submission.
7.  **Resolution & Outcomes:**
    *   **You Win:** The disputed amount is returned to you. The chargeback fee *may* be refunded depending on your country/region.
    *   **You Partially Win:** A portion of the disputed amount is returned. The fee refund policy still applies.
    *   **Cardholder Wins:** Neither the disputed amount nor the fee is returned. The decision is final.

### **2.2. Inquiry Process Flow**

1.  **Initiation:** The cardholder disputes a charge with their bank.
2.  **Evidence Request:** The issuing bank sends an inquiry request for more information. **No funds are withdrawn.**
3.  **Response Window:** You have a limited time to respond.
4.  **Evidence Submission:** You submit evidence or resolve the issue directly (e.g., by issuing a refund).
5.  **Review:** The credit card company reviews the evidence. This can take 65-75 days after the transaction date.
6.  **Resolution & Outcomes:**
    *   **Closed in Your Favor:** The case is closed. No money changes hands.
    *   **Cardholder Wins:** The inquiry is escalated to a full **Chargeback**. The disputed amount and fee are then withdrawn immediately (Return to Section 2.1, Step 2).

---

## **Section 3: Response Strategy & Execution**

Upon receiving a dispute notification, choose one of the three strategic paths.

### **3.1. Path A: Fight the Dispute (Submit Evidence)**

This is the path for disputes you believe are invalid.

1.  **Identify the Reason:** Check the chargeback reason code in Shopify Admin (e.g., "Fraudulent," "Product not received").
2.  **Gather Evidence:** Collect evidence based on the specific reason. Refer to the **Evidence Matrix in Section 4**.
3.  **Format Evidence Correctly:**
    *   Use high-contrast images and documents (e.g., black and white PDFs).
    *   Ensure documents are legible without zooming/cropping. Many banks still use fax machines.
    *   **Do not use links** as evidence; they will be ignored.
4.  **Submit Response:** Add all evidence to the chargeback response form in the Shopify Admin and click **Submit response** before the deadline.

### **3.2. Path B: Resolve with the Customer Directly**

This path aims to have the customer withdraw the dispute.

1.  **Contact Customer:** Reach out via phone or email to understand the issue.
2.  **Find a Resolution:** If you reach an agreement, the customer **must contact their bank** to cancel the dispute.
3.  **Obtain a Withdrawal Letter:** This is **CRITICAL**. The customer must get a formal withdrawal letter from their bank and send it to you. This letter must include:
    *   Official bank letterhead
    *   Case number
    *   Original charge date and amount
    *   Your store/business name
    *   Confirmation that the chargeback was canceled and funds were returned to you.
4.  **Submit Evidence:** You **must still submit a response** to the chargeback. The primary piece of evidence will be the withdrawal letter.
5.  **Do NOT Refund Immediately:** Wait until the chargeback status is fully resolved in your Shopify Admin before issuing any promised refund. This can take 30-90 days.

### **3.3. Path C: Accept the Dispute**

This is the path for disputes you agree are valid.

*   **For a Chargeback:** You can accept it by simply not submitting any evidence. The funds and fee will not be returned.
*   **For an Inquiry:** You can end the process by issuing a **full refund** for the order. This prevents it from escalating to a chargeback. You should still submit proof of the refund as evidence in the inquiry response.
    *   **Warning:** Issuing a *partial* refund during an inquiry will not prevent a full chargeback.

---

## **Section 4: Evidence Matrix by Dispute Reason**

Use this table to gather the strongest evidence for your case.

| Dispute Reason | Definition | Recommended Evidence to Submit |
| :--- | :--- | :--- |
| **Fraudulent** / **Unrecognized** | Cardholder claims they did not authorize the charge. | - **Shopify Fraud Analysis** (with AVS/CVV match info). <br>- Proof of delivery with tracking number and recipient address. <br>- IP address, timestamp, and billing information used for the order. <br>- Any communication with the customer. |
| **Product not Received** | Customer claims they never received the purchased goods/services. | - **Proof of Delivery (POD):** Tracking number showing "delivered" status to the correct address is strongest. <br>- Shipping confirmations, customer's billing information. <br>- For digital goods: Activity logs showing the customer accessed the product/service. |
| **Product Unacceptable** | Product was defective, damaged, or not as described. | - Proof of delivery (to show it was received). <br>- Photos/descriptions from your store page proving the product was as described. <br>- Evidence that the customer did not attempt a return before the chargeback. <br>- Any communication offering a replacement or resolution. |
| **Duplicate** | Customer believes they were charged twice for the same item. | - Receipts for both transactions proving they were for separate products or services. <br>- An explanation of why there were two distinct charges. |
| **Subscription Canceled** | Customer claims they were charged after canceling a recurring subscription. | - Your subscription cancellation policy. <br>- Proof of where/when the policy was shown to the customer. <br>- Communication with the customer about their cancellation (e.g., confirmation email). <br>- Activity logs showing service access *after* they claim to have canceled. |
| **Credit not Processed** | Customer claims they returned an item or canceled a service but were not refunded. | - Your refund/return policy. <br>- An explanation of why the customer was not entitled to a refund (if applicable). <br>- Communication with the customer about the return/refund status. |
| **General** | A catch-all category for disputes that don't fit others. | - A comprehensive collection of all relevant evidence: product details, fulfillment date/time, customer billing/IP info, all communication, and POD. |

---

## **Section 5: Prevention Strategy Matrix**

Proactively reduce the risk of chargebacks.

| Dispute Reason | Prevention Tactics |
| :--- | :--- |
| **Fraudulent** / **Unrecognized** | - Set a clear, recognizable **billing statement descriptor** in Shopify Payments (e.g., "YourStoreName.com"). <br>- Use Shopify's fraud analysis tools. Be wary of orders with multiple AVS/CVV mismatches. <br>- Send immediate order confirmation receipts. |
| **Product not Received** | - Ship orders promptly and use carriers that provide reliable tracking and delivery confirmation. <br>- Proactively communicate any shipping delays to the customer. |
| **Product Unacceptable** | - Use high-quality, accurate product photos and detailed descriptions. <br>- Pack items securely to prevent damage in transit. <br>- Maintain a clear and fair return policy and respond to complaints quickly. |
| **Duplicate** | - If you accidentally double-charge, refund one charge immediately and notify the customer. <br>- Ensure receipts for similarly priced items are distinct and clear. |
| **Subscription Canceled** | - Have a clear, easily accessible subscription policy. <br>- Process cancellation requests immediately and send a confirmation email. <br>- Be transparent about recurring charges on the sign-up page. |
| **Credit not Processed** | - Post a clear and fair return policy on your store. <br>- Process eligible refunds promptly upon receiving returned items. |
