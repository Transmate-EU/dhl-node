# dhl-node

A node client that implements DHL Express Global Web Services which is based on SOAP.

The web services are documented in [DHL_Express_Global_Web_Services_-_Developer_Guide_V3.1.pdf](doc/DHL_Express_Global_Web_Services_-_Developer_Guide_V3.1.pdf) and [Reference_Data.xlsx](doc/Reference_Data.xlsx) contains the valid values of various fields.

This client implements the `RateRequest`, `ShipmentRequest`, and `TrackingRequest` requests. The `ShipmentDeleteRequest` and `DocumentRetrieve` requests are not implemented by this client, but they should be trivial to add.

## Authentication

DHL provides a test account and a live account when giving access. Both of these accounts have an associated username, password, and an account number. You can copy `auth.sample.js` as `auth.js`, and replace its values with the values of your test account to be able to use the scripts of this repo.

