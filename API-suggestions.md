# Introduction
The purpuse of this document is to define a new product at LTS AS.

# Nomenclature
TLA | Description
------------ | -------------
PDF | Document in PDF format
API | Application programming interface
OTP | One-time passcode from a Yubikey

# PDF review product
## Customers API-calls
- order(spesification, product, customer_signature, SHA2)
- ack(task_ID)
- ack(task_ID, timestamp_for_planned_delivery)
- delivery(spesification_report, product_report, reviewer_signature, SHA2)

## Reviewers API-calls
- request(order_ID)
- ack(order_ID, timestamp_for_planned_delivery)
- order(PDF, customer_OTP, SHA2)
- delivery(PDF, reviewer_OTP, SHA2)

## Proccess
- [ ] Verify order checksum
- [ ] Verify customer_OTP
- [ ] Save PDF in workspace
- [ ] Send first ack
- [ ] Allocate task in users calendar
- [ ] Send timestamp_for_planned_delivery
- [ ] Move PDF to reviewers workspace
- [ ] Verify delivery checksum
- [ ] Verify reviewer_OTP
- [ ] Send delivery to customer
- [ ] Add line to monthly invoice
