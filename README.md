# SmartCart

SmartCart is a browser-based shopping assistant and shopping-list planner. This repository contains both the project website and **the actual SmartCart application**.

- [`index.html`](./index.html) is the project website, which introduces SmartCart and links to more information.
- [`smartcart.html`](./smartcart.html) is the working shopping assistant application.

You can visit the website online [here](https://booksareverycool-lang.github.io/smartcart).

## Features

- Browse, search, and filter the sample store catalogue.
- Add and remove products, choose quantities and product options, and manage a shopping list.
- Track an estimated total, savings, and budget.
- Compare products, explore suggestions, and view an aisle map.
- Optionally use the Gemini-powered assistant to find products and build a list.

Catalogue prices, nutrition, ingredients, and store information are demo estimates. They are not live inventory or verified product data.

## Run the application

The app is a standalone HTML file with no build step or package installation required. Open `smartcart.html` in a modern browser. The catalogue, list, filters, budget, comparisons, and aisle map work locally in the browser.

## Set up the AI assistant

The optional AI shopping assistant requires **your own Gemini API key**:

1. Create a key in [Google AI Studio](https://aistudio.google.com/app/apikey).
2. Open `smartcart.html` and replace the `GEMINI_API_KEY` placeholder near the top of its script with your key.
3. Save the file and reload it in your browser.

Do not publish or commit your personal key. This app calls Gemini directly from the browser, which means a key added to the HTML can be viewed by anyone who gets that copy of the file. For a public or production deployment, make API requests through a backend that keeps the key private.

## Technology

The application is implemented in a single HTML file with inline CSS and JavaScript. The optional assistant uses the Gemini API, and the page loads typography from Google Fonts.
