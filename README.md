# Amazon India TV Scraper

A Node.js web scraper that extracts detailed product information from Amazon India's smart TV listings.

## Features

- Extracts comprehensive product details including:
  - Product name and specifications
  - Ratings and reviews
  - Pricing and discounts
  - Bank offers
  - Product images
  - Technical specifications
  - AI-generated review summaries

## Technologies Used

- Node.js
- Puppeteer (for dynamic content)
- Cheerio (for HTML parsing)
- Axios (for HTTP requests)

## Installation

1. Clone the repository:
```bash
git clone https://github.com/samalasripadh/assignment.git
cd assignment
```

2. Install dependencies:
```bash
npm install
```

## Usage

1. Run the scraper:
```bash
node smartTVScraper.js
```

2. Enter the Amazon product URL when prompted

3. The scraped data will be saved in the `scraped_data` directory as a JSON file

## Data Structure

The scraper saves data in the following format:
```json
{
  "productName": "string",
  "rating": "string",
  "numberOfRatings": "string",
  "sellingPrice": "string",
  "mrp": "string",
  "totalDiscount": "string",
  "bankOffers": [],
  "aboutThisItem": {},
  "productInfo": {},
  "productImages": [],
  "manufacturerImages": [],
  "aiSummary": "string",
  "url": "string",
  "scrapedAt": "ISO date string"
}
```

## Error Handling

- Implements anti-bot detection measures
- Handles verification pages
- Includes retry mechanisms
- Validates extracted data
