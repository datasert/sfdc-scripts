# Overview
This repository stores the commonly used soql queries related to Standard objects.

Hope is that this would be a start point for somebody to use these to build on new ones per their needs.

# Types of content
Content supports various types of content. As of now, it is `soql` and `sosl`.

# Format
Content is maintained in `content.json` in json format. Each entry must be added to root object with `category` and list of items.

# Scripts

## Account
### Accounts created today
(soql) Shows the list of accounts created today

```select id, name, parent.name, billingstreet, billingcity, billingstate, billingpostalcode from account where createddate = today```
