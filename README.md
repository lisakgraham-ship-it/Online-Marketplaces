# Online Marketplaces: Photo to Listing

Upload a photo of something you want to sell. Claude identifies it, researches
current US resale prices, and writes a recommended price, title, and
description for **Facebook Marketplace** and **Vinted**. You review the result,
ask for fixes if something is off, then copy it into each site and publish it
yourself.

Based on the `crosslist-content-generator` skill.

## Use it

Open `index.html` in a browser, or (once GitHub Pages is on) visit the site
link. Then:

1. Create an Anthropic API key at <https://console.anthropic.com/settings/keys>
   (add a few dollars of credit; each listing costs a few cents).
2. Paste the key into the app and click **Save key**. It is stored only in your
   browser and sent only to Anthropic. Each person (family members included)
   uses their own key.
3. Add 1-5 photos and any notes ("brand new", "size 8"), then click
   **Create my listing**.
4. If something is wrong, type what to change under **Something not right?**
   and click **Update listing**.
5. Use the **Copy** buttons to paste each field into Facebook Marketplace or
   Vinted.

## Share it

Turn on GitHub Pages: repo **Settings > Pages > Build and deployment >
Source: Deploy from a branch > main / (root)**. Share the link GitHub shows.

The repo is public, so never commit an API key. The app never stores keys on
any server.

## Notes

- Vinted is only for clothing, shoes, accessories, and home textiles. The app
  skips it for other items and says why.
- Prices are estimates from web search results. Check the comparable listings
  shown before you post.

## Roadmap

- Phase 2 (experimental): a helper that opens Facebook Marketplace and Vinted
  in your own browser and fills in a draft, stopping before Publish.
