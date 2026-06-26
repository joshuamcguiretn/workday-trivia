# Workday Trivia — Live Checkout Setup Runbook

Purpose: turn the completed Workday Trivia Year Edition package into a real paid checkout without rethinking the offer.

Current state:
- Product inventory is complete: 52 presenter decks, 52 host guides, and bonus tools.
- Launch delivery format is native Google Slides and Google Docs.
- Public website currently supports request-access/manual follow-up, not instant paid checkout.
- Build Mode cannot exit until checkout and delivery are verified end-to-end.

## Recommended checkout provider

Use Payhip or Gumroad. Pick whichever account is already easiest for Joshua to access.

Do not keep comparing providers. The priority is to create one functioning paid product and test delivery.

## Product setup fields

Product title:
Workday Trivia Year Edition — 52 Ready-to-Run Team Trivia Rounds

Price:
$299 one-time payment

Product type:
Digital product / digital download / external access product

License:
One manager-led team or recurring group. Internal use only. No resale, redistribution, public posting, or repackaging.

Support email:
joshua.mcguire.tn@gmail.com

## Product description

Use the copy in:
checkout/payhip-listing-copy.md

Do not rewrite the offer during setup unless the checkout platform requires shorter copy.

## Fulfillment option A — preferred

Use this if the customer package folder can be shared safely:

1. Open the Workday Trivia Year Edition customer package folder in Google Drive.
2. Confirm the package contains:
   - 00-Start-Here
   - 01-Presenter-Decks
   - 02-Host-Guides-and-Answer-Sheets
   - 03-Bonus-Tools
3. Set the folder share permission to either:
   - Anyone with the link can view, or
   - restricted access with buyer email added manually after purchase.
4. Put the package access link in the checkout fulfillment message.
5. Complete one test purchase using a non-owner/buyer email.
6. Confirm the buyer can open the Start Here folder and at least one presenter deck and host guide.

## Fulfillment option B — fallback

Use this if Joshua does not want the whole folder publicly accessible:

1. Checkout provider sends buyer this message after purchase:

Thanks for buying Workday Trivia Year Edition.

Your purchase includes 52 ready-to-run workplace trivia rounds, presenter decks, host guides, answer sheets, and bonus tools in native Google Slides and Docs format.

Your files are delivered by Google Drive access. Reply to this purchase email with the Google account you want access granted to, or email joshua.mcguire.tn@gmail.com from the purchase email.

Recommended first step after access is granted: open the Start Here folder and read the Quick Start / Final Package Audit checklist.

2. Joshua grants Drive folder access to the buyer email.
3. Joshua replies with the folder link.
4. Track first buyer friction; if two or more buyers are confused, switch to a more automated access method.

## Website update after checkout is live

After the checkout URL exists:

1. Replace the main CTA in index.html from `early-access.html` to the real checkout URL.
2. Replace the form CTA in early-access.html with either:
   - a primary button to the real checkout, or
   - a secondary request-access form for invoice/custom licensing.
3. Keep the free starter pack CTA in place.
4. Do not move to Growth Mode until the live checkout URL and buyer access path are tested.

## End-to-end test checklist

- Product page opens publicly.
- Price displays as $299.
- License terms are visible before purchase or in fulfillment copy.
- Test purchase/payment completes.
- Confirmation email is received.
- Buyer receives either direct package access or clear access-request instructions.
- Buyer account can open package folder.
- Buyer account can open one deck.
- Buyer account can open one host guide.
- Buyer account can find Start Here instructions.
- Website CTA points to the live checkout URL.

## Build Mode exit rule

Only exit Build Mode when:

1. Overall readiness remains 80/100 or higher.
2. All 52 weeks remain complete and package-ready.
3. The live checkout/delivery path has been verified end-to-end.

At that point, update Agent 4 to Growth Mode and focus on traffic, conversion, feedback, and sales improvement.
