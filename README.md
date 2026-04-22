# BTR Sports — Product Feed for Affiliates

Public product feed for [btrsports.co.uk](https://btrsports.co.uk). All active, in-range products in whichever format suits you. Refreshed automatically but contact us if you need a particular update pushed.

## Download

| Format | URL |
|---|---|
| CSV  | [affiliate-feed.csv](https://raw.githubusercontent.com/web3at50/btr-feed/main/affiliate-feed.csv) |
| JSON | [affiliate-feed.json](https://raw.githubusercontent.com/web3at50/btr-feed/main/affiliate-feed.json) |
| XML (Google Shopping / RSS 2.0) | [affiliate-feed.xml](https://raw.githubusercontent.com/web3at50/btr-feed/main/affiliate-feed.xml) |

All three URLs are stable — they will always point to the latest version.

## Fields

| Field | Description |
|---|---|
| `sku` | BTR product SKU (e.g. `BTR294`) |
| `title` | Product name |
| `summary` | Short product description (~240 chars) |
| `price_gbp` | Retail price in GBP |
| `product_url` | Direct link to the product page on btrsports.co.uk |
| `image_url` | Hosted product image on Shopify's CDN (800px wide) |
| `image_alt` | Alt text for the image where available |
| `vendor` | Brand (BTR Sports) |
| `product_type` | Product category |
| `in_stock` | `yes` / `no` at time of feed generation |

In the XML feed, fields are mapped to the standard [Google Merchant](https://support.google.com/merchants/answer/7052112) schema (`g:id`, `g:title`, `g:description`, `g:link`, `g:image_link`, `g:price`, `g:availability`, `g:brand`, `g:product_type`, `g:condition`).

## Using the images

Images are served from Shopify's CDN and are safe to hotlink directly — no need to download or re-host them. Need a different size? Append or change the `width=` query parameter:

```
...product-image.jpg?width=400    (thumbnail)
...product-image.jpg?width=800    (default — product card)
...product-image.jpg?width=1200   (hero / zoom)
```

## Affiliate programme

BTR partners get:

- 15% Commission on referred sales
- Custom tracked referral link
- Optional banner assets on request

Managed via [GoAffPro](https://goaffpro.com). To join, contact us and we'll set you up end-to-end — you just need to share your link and code. 

Or signup yourself here: https://btrsports.goaffpro.com/create-account

## Contact

Email **bryn@btrdirect.co.uk** for affiliate sign-up, custom feed formats or any questions.

---

_Last generated: see git commit history above._
