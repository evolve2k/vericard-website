---
title: Developers
discover:
  title: Developers
permalink: /developers/index.html
description: Information for Developers
layout: page
---

`This area is under active development. These instructions are not yet finalised.`

Per Australian regulations, Social Media Providers are required to enable age verification solutions.

How to use our service.

1. Go here to [register for API access](https://vericard.digital/providers/register)
2. Embed our 'Age Verification Check' into your service
3. Record the outcome of age verification in your system.

Internally we record that you undertook a verification and the result of that verification, we expect to keep these logs for 90 days. The log cannot be used to identify the end user, but we expect that an audit of our security process will show that what is provided to you is a valid age assessment.

### The full process - How it works for users

Once you are registered with us, you can add our service to your age verification providers, for most providers you'll implement an interface something like this:

Please select an age verification provider:
Vericard
Others..

Open our /verify site in an iframe.

Returned

vericard-verification {
	receipt_id: 34534235454235,
     provided_at:  Fri 31 Oct 2025 12:00:36 ACDT,
	over16: true
}

As instructed the user will check their app and provide a assurance code.
If the assurance code is valid, we'll return a 200 along with a receipt_id. The receipt id can be used for 180 days and just resends the information returned in the verify. The receipt will return if the age is valid or not but by design (for user privacy) cannot be used to link back to the user within our systems.

### Pricing

For entities that expect to do less than 6,000 verifications in any rolling six month period, there is currently no charge for our service. 
For larger social media providers, please contacts us via email.












