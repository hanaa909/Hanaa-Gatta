# The price is the page

Booking iteration for the Bitcoin Boost ticket. Price and order type lead the screen. Market shows the price you will get. Limit shows the price you are willing to pay.

Figma: [The price is the page](https://www.figma.com/design/hyJfx8LzlOJtyZU9PEgbLk/Nemo--%3E-UX?node-id=42510-2382)

The screens are on the **cursors designs** page in Nemo → UX.

## Screens

- **Market.** The number is **$100,000**, the best price available right now. The action is **Buy at $100,000**.
- **Limit.** The number is **$99,200**, which is **$800 under the market**. The action is **Place limit at $99,200**.

Market and Limit sit under the price as the decision. Amount, boost, and protection stay in the sheet below, using the existing inputs, toggles, and primary button.

## Color tokens

Colors on the new frames use the Nemo Color collection instead of raw values.

- Stage background: `Background/BG Primary`
- Sheet: `Background/BG Secondary`
- Boost row and idle order type: `Background/BG Card`
- Selected order type: `Color/Base/White`
- Price and titles: `Text/Primary`
- Supporting lines: `Text/Secondary` and `Text/Tertiary`
- Text on the selected type: `Text/Black`
- Amount label and value: `Components/Input/Text-Label` and `Components/Input/Text-Value`
- Outlines: `Components/Input/Border-Default`
