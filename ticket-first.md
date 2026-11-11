# Ticket first

Iteration 2 of the Buy screen in the extended hours flow. Order type and the ticket price move to the top of the screen. You pick Market or Limit first, see what one share costs (or set your limit), and then decide how much to invest.

Figma: [Ticket first — iteration 2](https://www.figma.com/design/hyJfx8LzlOJtyZU9PEgbLk/Nemo--%3E-UX?node-id=42536-2141)

Source screens: [Extended hours, regular session flow](https://www.figma.com/design/hyJfx8LzlOJtyZU9PEgbLk/Nemo--%3E-UX?node-id=42436-6180)

Prototype: [prototypes/ticket-first.html](prototypes/ticket-first.html), also published at https://claude.ai/artifact/UCXzfKvF65Y1uUZ7ChW5Ae (private until shared).

## What changed

- A **Ticket** card sits directly under the Buy Apple header.
  - **Order type** comes first. The existing Market and Limit chips become a full-width switch.
  - **Ticket price** comes second, in large type.
- **Market** shows "Market price · per share", **$276.87**, and a line saying you pay the best price available when the order executes.
- **Limit** moves the existing limit price field from the bottom of the card to the ticket. It shows **$270.00**, "$6.87 below the current price", the current price, and "Your order only fills if Apple trades at $270.00 or lower."
- The amount card follows the ticket. It keeps the investment bar, the shares and USD inputs, and the Extended hours toggle.
- Removed because the ticket now covers them: the "1 APPL = $173.00" header line, the "Invest now at…" and "Choose the quantity and the price…" lines, and the price row on Limit.
- The Limit button reads **Review limit order**.

## Prototype

The prototype covers:

- Switching between Market and Limit.
- Market: entering USD or shares, with a live estimate and an over-balance error.
- Limit: typing a price, using + / −, or picking −5%, −2%, −1% or the current price. A limit above market shows a warning.
- The first-time Extended hours explainer, with the required acknowledgement.
- Review and confirmation for both order types.

## Built from

The Figma screens are copies of the original Market and Limit screens, so they keep the Nemo App (Master) components. The new ticket card uses library tokens.

- Card: `Background/BG Card`, `radius-xl`, `Card/padding-md`, `spacing-md`
- Order type track: `Background/BG Secondary`, `radius-full`
- Price: `Heading/Heading 2`, `Text/Primary`
- Labels and explainers: `Body Medium/Regular`, `Body Small/Regular`, `Text/Tertiary`
- Limit field outline: `Components/Input/Border-Active`

## Open questions

- The source screens disagree on the price ($173.00 in the header, $276.87 as the current price). This iteration uses $276.87.
- The order type track uses `Background/BG Secondary` because `Color/White (alpha)/20` doesn't import from the library. The contrast against the card is low.
- The pre-market flow isn't updated yet.
