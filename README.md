# payment
curl https://api.stripe.com/v1/charges/ch_1HCdAXCt0wO1R3UBvKO74yZg \
  -u sk_test_51HCKUsCt0wO1R3UB0KjHsRsQMAlbzd4IHbVUbVqOWFJPop66PfSSuQbQ0Q5bUuFL5aPQqokLMsVvqmScEgIOoR2n00WjC81ugp: \
  -d "expand[]"=customer \
  -d "expand[]"="invoice.subscription" \
  -G
  
  
  {
  "id": "ch_1HCdAXCt0wO1R3UBvKO74yZg",
  "object": "charge",
  "amount": 100,
  "amount_refunded": 0,
  "application": null,
  "application_fee": null,
  "application_fee_amount": null,
  "balance_transaction": "txn_1HCdAXCt0wO1R3UBhBeWTBMk",
  "billing_details": {
    "address": {
      "city": null,
      "country": null,
      "line1": null,
      "line2": null,
      "postal_code": null,
      "state": null
    },
    "email": null,
    "name": "Jenny Rosen",
    "phone": null
  },
  "calculated_statement_descriptor": null,
  "captured": false,
  "created": 1596597597,
  "currency": "jpy",
  "customer": null,
  "description": "My First Test Charge (created for API docs)",
  "disputed": false,
  "failure_code": null,
  "failure_message": null,
  "fraud_details": {},
  "invoice": null,
  "livemode": false,
  "metadata": {
    "order_id": "6735"
  },
  "on_behalf_of": null,
  "order": null,
  "outcome": null,
  "paid": true,
  "payment_intent": null,
  "payment_method": "card_1HCbvSCt0wO1R3UBX5AET2vU",
  "payment_method_details": {
    "card": {
      "brand": "visa",
      "checks": {
        "address_line1_check": null,
        "address_postal_code_check": null,
        "cvc_check": "pass"
      },
      "country": "US",
      "exp_month": 8,
      "exp_year": 2021,
      "fingerprint": "dEokqYuLj5tQfjqX",
      "funding": "credit",
      "installments": null,
      "last4": "4242",
      "network": "visa",
      "three_d_secure": null,
      "wallet": null
    },
    "type": "card"
  },
  "receipt_email": null,
  "receipt_number": null,
  "receipt_url": "https://pay.stripe.com/receipts/acct_1HCKUsCt0wO1R3UB/ch_1HCdAXCt0wO1R3UBvKO74yZg/rcpt_HmBXEeXOmFllyKd1BwBK1fwPJ12PxsR",
  "refunded": false,
  "refunds": {
    "object": "list",
    "data": [],
    "has_more": false,
    "url": "/v1/charges/ch_1HCdAXCt0wO1R3UBvKO74yZg/refunds"
  },
  "review": null,
  "shipping": null,
  "source_transfer": null,
  "statement_descriptor": null,
  "statement_descriptor_suffix": null,
  "status": "succeeded",
  "transfer_data": null,
  "transfer_group": null
}
