# wooLocalCheckoutFields
Plugin to adapt to the needs per country instead of just letting users fill in the two address fields.

# Goals:
1. Change the checkout page to meet the needs per country
2. Use these customized fields to set the two address fields. 

# Example case:
In The Netherlands there is no such thing as a seconds address line. If we need to write down our address, we need these fields:
* streetname
* housenumber
* optional addition to housenumber

The goal is to ask these fields to the user. And then put them in WooCommerce address_1 as:
<streetname> <housenumber> <addition>

That is what the correct format should be on a Dutch (Netherlands) address. 

# Why put it in address_1 ?
A lot of plugins, fulfilment parties and shipping label companies trust on the two default address fields of WooCommerce. That's why I don't want to add custom fields, I only want to ask custom fields to improve the user experience and then use those fields to set the value of address_1 and/or address_2. This depends per country.
