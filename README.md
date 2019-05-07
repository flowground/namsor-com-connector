# ![LOGO](logo.png) NamSor API v2 **flow**ground Connector

## Description

A generated **flow**ground connector for the NamSor API v2 API (version 2.0.2-beta).

Generated from: https://api.apis.guru/v2/specs/namsor.com/2.0.2-beta/openapi.json<br/>
Generated at: 2019-05-07T17:43:07+03:00

## API Description

NamSor API v2 : enpoints to process personal names (gender, cultural origin or ethnicity) in all alphabets or languages. Use GET methods for small tests, but prefer POST methods for higher throughput (batch processing of up to 1000 names at a time). Need something you can't find here? We have many more features coming soon. Let us know, we'll do our best to add it! 

## Authorization

Supported authorization schemes:
- API Key
## Actions

### List of API services and usage cost in Units (default is 1=ONE Unit).

*Tags:* `admin`

### Print current API usage.

*Tags:* `admin`

### Print historical API usage.

*Tags:* `admin`

### Print historical API usage (in an aggregated view, by service, by day/hour/min).

*Tags:* `admin`

### List all available plans in the default currency (usd).

*Tags:* `admin`

### List all available plans in the user's preferred currency.

*Tags:* `admin`

#### Input Parameters
* `token` - _required_

### List possible currency options for billing (USD, EUR, GBP, ...)

*Tags:* `admin`

### Read the history billing information (invoices paid via Stripe or manually).

*Tags:* `admin`

#### Input Parameters
* `token` - _required_

### Read the billing information (company name, address, phone, vat ID)

*Tags:* `admin`

#### Input Parameters
* `token` - _required_

### Create a Stripe Customer, based on a payment card token (from secure StripeJS) and email.

*Tags:* `admin`

### Identify Chinese name candidates, based on the romanized name.

*Tags:* `chinese`

#### Input Parameters
* `chineseSurnameLatin` - _required_
* `chineseGivenNameLatin` - _required_

### Identify Chinese name candidates, based on the romanized name (firstName = chineseGivenName; lastName=chineseSurname).

*Tags:* `chinese`

### Identify Chinese name candidates, based on the romanized name (firstName = chineseGivenName; lastName=chineseSurname).

*Tags:* `chinese`

### Identify Chinese name candidates, based on the romanized name - having a known gender ('male' or 'female')

*Tags:* `chinese`

#### Input Parameters
* `chineseSurnameLatin` - _required_
* `chineseGivenNameLatin` - _required_
* `knownGender` - _required_

### Setting an API Key to a corporate status.

*Tags:* `admin`

#### Input Parameters
* `apiKey` - _required_
* `corporate` - _required_

### [USES 10 UNITS] Infer the likely country of residence of a personal full name, or one surname. Assumes names as they are in the country of residence OR the country of origin.

*Tags:* `personal`

#### Input Parameters
* `personalNameFull` - _required_

### [USES 10 UNITS] Infer the likely country of residence of up to 1000 personal full names, or surnames. Assumes names as they are in the country of residence OR the country of origin.

*Tags:* `personal`

### Update debug level for a classifier

*Tags:* `admin`

#### Input Parameters
* `logger` - _required_
* `level` - _required_

### [USES 20 UNITS] Infer the likely ethnicity/diaspora of a personal name, given a country of residence ISO2 code (ex. US, CA, AU, NZ etc.)

*Tags:* `personal`

#### Input Parameters
* `countryIso2` - _required_
* `firstName` - _required_
* `lastName` - _required_

### [USES 20 UNITS] Infer the likely ethnicity/diaspora of up to 1000 personal names, given a country of residence ISO2 code (ex. US, CA, AU, NZ etc.)

*Tags:* `personal`

### Infer the likely gender of a name.

*Tags:* `personal`

#### Input Parameters
* `firstName` - _required_
* `lastName` - _required_

### Infer the likely gender of up to 1000 names, detecting automatically the cultural context.

*Tags:* `personal`

### Infer the likely gender of a full name, ex. John H. Smith

*Tags:* `personal`

#### Input Parameters
* `fullName` - _required_

### Infer the likely gender of up to 1000 full names, detecting automatically the cultural context.

*Tags:* `personal`

### Infer the likely gender of a full name, given a local context (ISO2 country code).

*Tags:* `personal`

#### Input Parameters
* `fullName` - _required_
* `countryIso2` - _required_

### Infer the likely gender of up to 1000 full names, with a given cultural context (country ISO2 code).

*Tags:* `personal`

### Infer the likely gender of a name, given a local context (ISO2 country code).

*Tags:* `personal`

#### Input Parameters
* `firstName` - _required_
* `lastName` - _required_
* `countryIso2` - _required_

### Infer the likely gender of up to 1000 names, each given a local context (ISO2 country code).

*Tags:* `personal`

### Invalidate system caches.

*Tags:* `admin`

### Activate/deactivate learning from a source.

*Tags:* `admin`

#### Input Parameters
* `source` - _required_
* `learnable` - _required_

### Get the overall API counter

*Tags:* `admin`

### [USES 10 UNITS] Infer the likely country of origin of a personal name. Assumes names as they are in the country of origin. For US, CA, AU, NZ and other melting-pots : use 'diaspora' instead.

*Tags:* `personal`

#### Input Parameters
* `firstName` - _required_
* `lastName` - _required_

### [USES 10 UNITS] Infer the likely country of origin of up to 1000 names, detecting automatically the cultural context.

*Tags:* `personal`

### Infer the likely first/last name structure of a name, ex. John Smith or SMITH, John or SMITH; John.

*Tags:* `personal`

#### Input Parameters
* `nameFull` - _required_

### Infer the likely first/last name structure of a name, ex. John Smith or SMITH, John or SMITH; John. For better accuracy, provide a geographic context.

*Tags:* `personal`

#### Input Parameters
* `nameFull` - _required_
* `countryIso2` - _required_

### Infer the likely first/last name structure of a name, ex. John Smith or SMITH, John or SMITH; John.

*Tags:* `personal`

### Infer the likely first/last name structure of a name, ex. John Smith or SMITH, John or SMITH; John. Giving a local context improves precision.

*Tags:* `personal`

### Infer the likely gender of up to 1000 fully parsed names, detecting automatically the cultural context.

*Tags:* `personal`

### Infer the likely gender of up to 1000 fully parsed names, detecting automatically the cultural context.

*Tags:* `personal`

### Get the Stripe payment information associated with the current google auth session token.

*Tags:* `admin`

#### Input Parameters
* `token` - _required_

### [USES 11 UNITS] Infer the likely country and phone prefix, given a personal name and formatted / unformatted phone number.

*Tags:* `social`

#### Input Parameters
* `firstName` - _required_
* `lastName` - _required_
* `phoneNumber` - _required_

### [USES 11 UNITS] Infer the likely country and phone prefix, of up to 1000 personal names, detecting automatically the local context given a name and formatted / unformatted phone number.

*Tags:* `social`

### [USES 11 UNITS] Infer the likely phone prefix, given a personal name and formatted / unformatted phone number, with a local context (ISO2 country of residence).

*Tags:* `social`

#### Input Parameters
* `firstName` - _required_
* `lastName` - _required_
* `phoneNumber` - _required_
* `countryIso2` - _required_

### [USES 11 UNITS] Infer the likely country and phone prefix, of up to 1000 personal names, with a local context (ISO2 country of residence).

*Tags:* `social`

### Procure an API Key (sent via Email), based on an auth token. Keep your API Key secret.

*Tags:* `admin`

#### Input Parameters
* `token` - _required_

### Redeploy UI from current dev branch.

*Tags:* `admin`

### Redeploy UI from current dev branch.

*Tags:* `admin`

#### Input Parameters
* `live` - _required_

### Subscribe to a give API plan, using the user's preferred or default currency.

*Tags:* `admin`

#### Input Parameters
* `token` - _required_

### Stop learning and shutdown system.

*Tags:* `admin`

### Get the current software version

*Tags:* `admin`

### Print basic source statistics.

*Tags:* `admin`

#### Input Parameters
* `source` - _required_

### Print basic system statistics.

*Tags:* `admin`

### Connects a Stripe Account.

*Tags:* `admin`

#### Input Parameters
* `scope` - _optional_
* `code` - _optional_
* `error` - _optional_
* `error_description` - _optional_

### Subscribe to a give API plan, using the user's preferred or default currency.

*Tags:* `admin`

#### Input Parameters
* `planName` - _required_
* `token` - _required_

### Sets or update the billing information (company name, address, phone, vat ID)

*Tags:* `admin`

#### Input Parameters
* `token` - _required_

### Modifies the hard/soft limit on the API plan's overages (default is 0$ soft limit).

*Tags:* `admin`

#### Input Parameters
* `usageLimit` - _required_
* `hardOrSoft` - _required_
* `token` - _required_

### Update the default Stripe card associated with the current google auth session token.

*Tags:* `admin`

#### Input Parameters
* `defautSourceId` - _required_
* `token` - _required_

### [USES 10 UNITS] Infer a US resident's likely race/ethnicity according to US Census taxonomy W_NL (white, non latino), HL (hispano latino),  A (asian, non latino), B_NL (black, non latino).

*Tags:* `personal`

#### Input Parameters
* `firstName` - _required_
* `lastName` - _required_

### [USES 10 UNITS] Infer up-to 1000 US resident's likely race/ethnicity according to US Census taxonomy.

*Tags:* `personal`

### [USES 10 UNITS] Infer a US resident's likely race/ethnicity according to US Census taxonomy, using (optional) ZIP5 code info. Output is W_NL (white, non latino), HL (hispano latino),  A (asian, non latino), B_NL (black, non latino).

*Tags:* `personal`

#### Input Parameters
* `firstName` - _required_
* `lastName` - _required_
* `zip5Code` - _required_

### [USES 10 UNITS] Infer up-to 1000 US resident's likely race/ethnicity according to US Census taxonomy, with (optional) ZIP code.

*Tags:* `personal`

### Get the user profile associated with the current google auth session token.

*Tags:* `admin`

#### Input Parameters
* `token` - _required_

### Verifies an email, based on token sent to that email

*Tags:* `admin`

#### Input Parameters
* `emailToken` - _required_

### Verifies an email, based on token sent to that email

*Tags:* `admin`

#### Input Parameters
* `emailToken` - _required_

### Vetting of a source.

*Tags:* `admin`

#### Input Parameters
* `source` - _required_
* `vetted` - _required_

## License

**flow**ground :- Telekom iPaaS / namsor-com-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
