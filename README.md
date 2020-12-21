# Billing Domain Model
_This is my attempt to model the domain of billing_
## Problem statement
The company provides some service(s) for their customers. Each customer is subscribed on particular set of services. Invoices are issued based on subscription payment cycle. As soon, as invoice is issued the system attempts charging a customer based on its configured payment method.

Invoice can be paid outside the system, in this case someone from staff should reflect this in the system specifying payment document(s) references and (optionally) specifying the invoice this payment is for. Therefore, the invoice can be paid partially, or one payment can cover several invoices. If invoice was not specified the system have to chose one automatically.

Any of already paid payment can be refunded to the customer by someone from stuff.

A system have to provide the following information:
- account current balance
- list of expired unpaid account's invoices
- list of account payments that sill in progress