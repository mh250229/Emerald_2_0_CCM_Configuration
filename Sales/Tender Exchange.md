## Tender Exchange

A Tender Exchange is used to exchange one tender for another (referred to as a payment and refund), one tender is a payment tender and the other is a refund tender.

There are various business motivations for Tender Exchange. For example:

* Cash Withdrawal services - the customer pays $100.00 with an EFT card, e.g., Visa Card and gets a refund of $100.00 in cash

* Tender correction – the customer pays $100.00 with cash, then requests to swap the payment method with a different payment mean, e.g., pay with Visa.

* Coinstar to Cash – customers exchange CoinStar vouchers for cash. Coinstar vouchers are vouchers issued in exchange for Coins at the CoinStar Kiosks located in Retailer’s stores.

Currently, only Cash, EFT, and Vouchers are supported in a Tender Exchange flow.

The following flows are based on the Emerald 2.0 base configuration. For definitions of the tenders, see the Tender section.

### Configuring a Tender Exchange – Tender Correction

The following example shows how to set up a Tender Exchange for a Tender Correction.

1. Browse to Sales/Tendering/Tender Exchange.
2. Click **+Add Tender Exchange**.
3. In the **ID** field enter the unique ID representing the tender exchange, e.g., 1.
4. In the **Name** enter the name of the Tender Exchange, e.g., TenderCorrection.  
    **Note:** A Tender Correction button must be added to the Tender Exchange POS menu.
5. In the **Minimum Amount** field enter 0 indicating any amount is accepted.
6. In the **Maximum Amount** field enter 0 indicating any amount is accepted.
7. In the **Multiples Of** field enter 0. This indicates any denomination of the defined tender is allowed.
8. From the **Pay with Tenders** drop-down list, select the checkboxes of each tender that can be used as the paying tender, i.e., 10, 11, 12 (based on Emerald Base Configuration).
9. From the **Refund Tenders** drop-down list, select the tenders that can be refunded as the refundable tender, i.e., 10, 11, 12 (based on Emerald Base Configuration).
10. Click **Save**.

### Configuring a Tender Exchange – Tender Withdrawal

The following example shows how to set up a Tender Exchange for a Tender Withdrawal.

1. Browse to Sales/Tendering/Tender Exchange.
2. Click **+Add Tender Exchange**.
3. In the **ID** field enter the unique ID representing the tender exchange, e.g., 2.
4. In the **Name** enter the name of the Tender Exchange, e.g., CashWithdrawal.  
    **Note:** A CashWithdrawal button must be added to the Tender Exchange POS menu.
5. In the **Minimum Amount** field enter 0 indicating any amount is accepted.
6. In the **Maximum Amount** field enter 0 indicating any amount is accepted.
7. In the **Multiples Of** field enter 0. This indicates any denomination of the defined tender is allowed.
8. From the **Pay with Tenders** drop-down list, select the checkboxes of each tender that can be used as the paying tender, i.e., 10, 11, 12, 13 (based on Emerald Base Configuration).
9. From the **Refund Tenders** drop-down list, select the tenders that can be refunded as the refundable tender, i.e., 1 (based on Emerald Base Configuration).
10. Click **Save**.

### Configuring a Tender Exchange – CoinStarToCash

The following example shows how to set up a Tender Exchange for a CoinsStar to Cash.

1. Browse to Sales/Tendering/Tender Exchange.
2. Click **+Add Tender Exchange**.
3. In the **ID** field enter the unique ID representing the tender exchange, e.g., 3.
4. In the **Name** enter the name of the Tender Exchange, e.g., CoinStarToCash.
**Note:** A CoinStarToCash button must be added to the Tender Exchange POS menu.
5. In the **Minimum Amount** field enter 0 indicating any amount is accepted.
6. In the **Maximum Amount** field enter 0 indicating any amount is accepted.
7. In the **Multiples Of** field enter 0. This indicates any denomination of the defined tender is allowed.
8. From the **Pay with Tenders** drop-down list, select the checkboxes of each tender that can be used as the paying tender, i.e., 81 (based on Emerald Base Configuration).
9. From the **Refund Tenders** drop-down list, select the tenders that can be refunded as the refundable tender, i.e., 1 (based on Emerald Base Configuration).
10. Click **Save**.
