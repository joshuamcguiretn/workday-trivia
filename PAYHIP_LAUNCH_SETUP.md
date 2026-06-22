# Workday Trivia — Payhip Launch Setup

## Decision

Use **Payhip** as the first paid-delivery platform for the Year Edition.

Why this fit is practical for Workday Trivia:

- The free plan has no monthly charge and supports unlimited products/revenue, with a transaction fee.
- It can securely deliver downloadable files immediately after payment and emails buyers their download page.
- It can accept card and PayPal payments, which keeps checkout simple for workplace buyers.
- It can host the product page itself or connect a checkout button to the existing GitHub Pages site.

Do **not** publish a checkout button until the Year Edition files actually exist and have been tested. A working free sample is better proof than a premature preorder page.

---

## Product listing to create

### Product name

**Workday Trivia: The Year Edition — 52 Ready-to-Run Team Trivia Rounds**

### One-line promise

A full year of five-minute, workplace-safe trivia meetings — with every round planned, hosted, and ready to run.

### Recommended first pricing test

- **Founding launch price:** $39
- **Later regular price:** $59

This is a starting test, not a permanent pricing decision. The founding price rewards early buyers while the full price keeps the product positioned as an annual manager resource rather than a single printable.

### Product description (paste into Payhip)

**Stop spending meeting time figuring out how to make the meeting less awkward.**

Workday Trivia: The Year Edition gives managers, supervisors, trainers, HR teams, and remote leaders **52 original five-question trivia rounds** designed to fit into a quick weekly huddle, staff meeting, classroom, or virtual call.

Every round is workplace-safe, easy to host, and made to create a few minutes of friendly energy without adding prep work to your week.

#### What you receive

- 52 completely original weekly trivia rounds
- Five questions per round, plus a tie-breaker
- Screen-ready presenter decks for in-person, hybrid, or remote teams
- Print-friendly host guides and answer keys
- Quick facts that help turn answers into conversation
- Team score sheets and simple host instructions
- A start-here guide for running your first round in minutes

#### Important

The four free Starter Pack rounds are **not** included in the paid Year Edition. Buyers receive 52 additional rounds with no repeats.

#### Best for

- Weekly staff huddles
- Team meetings
- New-hire training groups
- Break rooms and shift changes
- Remote-team calls
- Leadership meetings that need a low-pressure warm-up

---

## Files that must be in the paid ZIP before launch

Create a private delivery ZIP outside this public GitHub repository.

```text
Workday-Trivia-Year-Edition.zip
├── START-HERE.pdf
├── LICENSE.txt
├── Week-01/
│   ├── Presenter-Deck.pdf
│   ├── Host-Guide-and-Answer-Key.pdf
│   └── Score-Sheet.pdf
├── Week-02/
│   └── ...
├── ...
└── Week-52/
    └── ...
```

Minimum quality gate before publishing:

1. All 52 rounds are present and unique.
2. Each round has exactly five questions, answer reveals, and one tie-breaker.
3. Every question has a verified answer and a brief, accurate fact or explanation.
4. PDFs open cleanly and print without layout breaks.
5. The free pack’s four rounds do not appear in the paid collection.
6. One person unfamiliar with the product can run a round using only `START-HERE.pdf`.

---

## Payhip setup steps that require account access

1. Create a Payhip store for Workday Trivia.
2. Connect a payout method (Stripe and/or PayPal).
3. Create a Digital Product using the name and description above.
4. Upload the final private ZIP.
5. Set the founding price at $39.
6. Add a clear product image and the free-starter-pack screenshot(s).
7. Test checkout with Payhip’s available preview/test flow before sharing it.
8. Copy the finished product URL.
9. Replace the Year Edition call-to-action in `index.html` with that product URL.

---

## Website button to add after the product URL exists

Replace `PASTE_PAYHIP_PRODUCT_URL_HERE` with the product URL:

```html
<a href="PASTE_PAYHIP_PRODUCT_URL_HERE" class="button primary">Get the 52-week Year Edition</a>
```

Place the button directly below the Year Edition checklist. Do not use a fake checkout link or an unavailable product button.

---

## Fast validation plan after checkout is live

Do not spend on ads first.

1. Share the free starter pack with 10 people who lead meetings, teams, classes, or volunteer groups.
2. Ask them to actually run one round.
3. Ask one question afterward: **“Would 52 original weekly rounds save you enough time to be worth $39?”**
4. Track:
   - number of people who opened the free pack
   - number who used at least one round
   - number who say yes to the price
   - exact wording of any hesitation
5. Fix only the repeating objections or usability issues; do not reopen broad redesign work.

---

## Access currently missing

The GitHub repository and website are accessible. Creating the store, connecting payments, uploading the private paid ZIP, and obtaining the product URL require the owner’s Payhip/Stripe/PayPal account access and cannot be completed from this repository alone.
