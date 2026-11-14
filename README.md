# Hi, I'm Ihab

I write Python backends, mostly for collecting data from websites and turning it into something people can use. Most of that is FastAPI, Postgres or SQLite, and scrapers that have to cope with real sites: rate limits, bot checks, and prices that only show up after JavaScript runs.

I also teach Python at Innokod.

## Projects

[box-price-intelligence](https://github.com/ihabND/box-price-intelligence) collects cardboard box prices from seven UK packaging suppliers every morning and works out who is cheapest at a given order quantity. Every supplier needed its own collector, from JSON embedded in product pages to Shopify endpoints to a Patchright browser for a site that renders its price tables client-side. I built it with two others; my part was the collectors, the comparison logic and the API.

[ihabov_universal_scraper](https://github.com/ihabND/ihabov_universal_scraper) is a scraping API. Send it a URL and it returns clean HTML, or JSON for sites it has a parser for. It tries plain HTTP first and switches to headless Chromium when a site blocks it. Redis holds the cache and the per-key quotas.

[captive-portal](https://github.com/ihabND/captive-portal) is the guest Wi-Fi login page for cafés. Each venue's OpenWRT router hands new guests to one FastAPI server that serves every venue, and a pair of shell scripts sets up a freshly flashed router.

## What I use

Python, FastAPI, SQLModel, Postgres, httpx, BeautifulSoup, Playwright and Patchright, Redis, Docker, pytest.

Most of my other repos are private: practice projects, university work and a couple of small Godot games.
