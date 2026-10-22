# AI Log — Exercise 1.9

## 1. What I Asked

I asked an AI tool: “Make me a simple one-page website in HTML for my tailoring shop in Serrekunda, The Gambia. Include what we do, our prices, our opening hours, and how to contact us.”

I then used the same prompt to generate a new page and wrote an improved prompt with explicit requirements for location, Gambian currency, opening hours, heading structure, important warnings, and avoiding unsupported business claims.

## 2. What I Got

The original AI-generated page contained HTML for a tailoring shop, but it also included business details that had not been provided, such as an establishment year, customer numbers, an award claim, prices in US dollars, contact details, and a deposit policy.

The new AI-generated pages differed in how they handled prices, opening hours, contact information, and uncertainty. The improved prompt produced a more structured page with prices and business details marked for confirmation. HTML validation helped check markup errors, but it could not verify whether business claims were true.

## 3. What I Changed and Why

In fixed-page.html, I added the language attribute and a meta description, and organized the content into semantic sections with a clear heading hierarchy.

I changed the prices to Gambian dalasi (GMD/D) and marked actual prices for the owner to confirm, because the real prices were not supplied.

I marked services and opening hours for confirmation instead of presenting unverified details as facts. I also highlighted Friday prayer hours as information the owner must confirm.

I replaced unverified phone numbers and email addresses with placeholders, removed unsupported claims about the shop's history, customer numbers, and awards, and marked the deposit policy for confirmation.

I used a proper list for the services and emphasized the order warning with `<strong>`. I also added comments identifying information that still needs confirmation before the website is published.