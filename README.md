# Homes.com (homes-com)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
