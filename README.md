# Homes.com (homes-com)

Homes.com is a United States residential real estate portal owned by CoStar Group, which acquired the property in 2021 and folded the Homesnap agent application into it — homesnap.com now issues an HTTP 301 to www.homes.com. It sits on the consumer-facing portal layer of the US housing value chain, alongside Zillow, Realtor.com, and Redfin: it aggregates for-sale, for-rent, and off-market listings sourced from Multiple Listing Services and broker syndication, and monetises through an agent-first advertising and agent-directory product rather than through data distribution. Its API posture is empty in both directions of the RESO question. Homes.com appears in the RESO organization directory as an active Technology Company (OrganizationUniqueId T00000143), but the Data Dictionary and Web API certification columns for that row are blank — it holds no RESO certification of any version, unlike rival Move/Realtor.com (Data Dictionary 1.7 Passed, Web API Core 2.0.0 Passed) or Zillow's Bridge Interactive (Data Dictionary 1.7 and Web API Core 2.0.0, Certified Legacy). Separately, no developer surface is published at all: developer., developers., api., docs., apis., dev., idx., feeds., and data. subdomains of homes.com do not resolve in DNS, and every path on www.homes.com returns HTTP 403 to non-browser clients behind Akamai bot protection. Listing data moves INTO Homes.com from MLSs and brokers via syndication opt-in, not OUT through any documented API.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/homes-com/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/homes-com/refs/heads/main/apis.yml)

## Tags

- Real Estate
- United States
- Property Listings
- MLS
- RESO
- IDX
- Rentals
- PropTech
- Portals
- Marketplaces
- Residential Real Estate
- Real Estate Agents
- Brokers
- Listings Syndication
- CoStar Group

## Timestamps

- **Created:** 2026-07-26
- **Modified:** 2026-07-26

## APIs

No first-party public APIs are published by Homes.com. The `apis` array is intentionally empty.

- **RESO posture:** Listed in the RESO organization directory as an active Technology Company (`T00000143`), with no Data Dictionary and no Web API certification recorded. Certification columns are populated for 25 of the 202 Technology Company rows in the same export, so the blank is a real absence, not a schema artefact.
- **Access gate:** `none-published`. There is no developer agreement, IDX/VOW licence, partner API application, or reseller path branded by Homes.com. Free self-serve agent web accounts exist — and MLS membership is explicitly not required for one — but they grant a directory profile in a browser, not an API credential.
- **Open data:** none.
- **Auth model:** none published. No `/.well-known/openid-configuration`, no API key programme, no OAuth or OIDC authorization server for third parties.
- **Webhooks / events / SDKs / Postman:** none first-party. The `Homesnap` and `CoStarGroup` GitHub organizations contain only archived forks of third-party libraries; the `libRETS` fork is a RETS *client* — evidence of consuming MLS feeds, not publishing them.

Third-party "Homes.com APIs" sold on RapidAPI, Apify, Parse, and RealtyAPI are unofficial scrapers and are deliberately not recorded here.

See [review.yml](review.yml) for the full probe table, HTTP statuses, and the verbatim RESO directory rows.

## Common Properties

- [Website](https://www.homes.com/)
- [About](https://www.homes.com/about/)
- [Support](https://support.homes.com/)
- [Blog](https://www.homes.com/blog/)
- [Terms Of Service](https://www.homes.com/about/homesterms-of-use)
- [Privacy Policy](https://www.homes.com/about/policies/#privacy-policy)
- [Accessibility](https://www.homes.com/about/accessibility/)
- [Contact](https://www.homes.com/about/contact-us/)
- [Sitemap](https://www.homes.com/sitemap/)
- [Parent](https://www.costargroup.com/)
- [Predecessor](https://www.homesnap.com/)
- [Standards Body](https://www.reso.org/certification/)
- [GitHub Organization](https://github.com/Homesnap)
- [LinkedIn](https://www.linkedin.com/company/homes-com)
- [Twitter](https://twitter.com/homesdotcom)
- [Facebook](https://www.facebook.com/homesdotcom)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
