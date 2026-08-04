# Shopping prompt review gates

Use these gates with the general method. Exact products, makers, patents, catalogue pages, prices, URLs, and outcomes remain in ignored local notes.

## Domain and time control

- Anchor the answer in a fixed historical sale record, catalogue, price list, advertisement, or order form rather than a current storefront.
- Freeze the season, year, edition, region, package size, shipping basis, and price type whenever they can change the answer.
- Ask for a price or product attribute printed in the source. Do not calculate inflation, tax, shipping, discounts, or unit price.

## Product identity

- Build product identity from independent maker history, patent, museum, or trade evidence before entering the catalogue.
- Keep model, capacity, action, maker, and year separate; a shared brand alone rarely selects one historical listing.
- Record every neighboring product with the same noun and its capacity, action, and price before promotion.
- Exclusions must remove real catalogue alternatives without revealing the target row or stock number.

## Terminal evidence and shortcuts

- Cite a direct human-viewable catalogue page or PDF page that visibly prints the product and requested price.
- Inspect the original page image; OCR snippets can reorder prices and descriptions across columns.
- Search natural combinations of model history, capacity, catalogue year, price wording, and proposed answer. Reject any result that exposes the complete product-price pair.
- Do not use current resale listings, collector estimates, search snippets, JSON, YAML, or arithmetic as final evidence.
- A candidate is ready only when at least two meaningful choices remain after the catalogue is found: the correct product row and the correct price type or neighboring variant.
