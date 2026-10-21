# Playwright Starter Kit

Three automated tests (login, cart, checkout) for the public practice site
https://www.saucedemo.com, written with Playwright and TypeScript.

## Requirements
- Node.js LTS (check with `node -v`)

## Run it
```bash
npm install
npx playwright install chromium
npm test
```

You should see 3 passing tests.

## See the report
```bash
npm run report
```

## Files
- `tests/login.spec.ts`: logs in with a valid user and checks the Products page.
- `tests/cart.spec.ts`: adds one product and checks the cart badge.
- `tests/checkout.spec.ts`: completes a purchase end to end.
- `playwright.config.ts`: browser, base URL and report settings.

## If a test fails
The practice site can change. Open the HTML report, check the screenshot,
then update the locator that no longer matches.
