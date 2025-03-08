
**Scraper ** is a Python application that scrapes data from three popular sources (Product Hunt, Hacker News, and SteamDB) and sends daily digests via email. Each source is handled by a dedicated scraper class, and the results are formatted into stylish HTML emails. The app can be run manually, scheduled, or compiled into a standalone executable for easy desktop use.

## Features

- **Product Hunt Scraper**: Fetches the 10 latest featured products from [Product Hunt](https://www.producthunt.com/) using the GraphQL API.
- **Hacker News Scraper**: Extracts the top 5 "Show" and "News" articles from [Hacker News](https://news.ycombinator.com/) based on upvotes.
- **SteamDB Scraper**: Collects the top 10 games from "Most Played," "Trending," "New Releases," and "Hot This Week" sections on [SteamDB](https://steamdb.info/) using Selenium.
- **Email Delivery**: Sends formatted HTML summaries to a configured email address.
- **Executable**: Can be compiled into a single `.exe` file for double-click execution or scheduling.

## Prerequisites

- **Python 3.8+**: Ensure Python is installed on your system.
- **Chrome Browser**: Required for Selenium (used by `SteamDBScraper`).
- **Gmail Account**: For sending emails via SMTP (requires an app password if 2FA is enabled).
