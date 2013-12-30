# node-comics-feed

RSS feeds of comics sites usually contains the links to a webpage but not the strip images. This module iterates on the items on a feed and parse the webpages to create a new feed with embedded comic strips.

Supported websites:
* GoComics
* Dilbert.com
> The list of parsers is meant to be extensible, see [`lib/parser.js`](lib/parsers.js). PR is welcome.

Inspired by [gocomics-scrape](https://github.com/mihaip/gocomics-scrape) and implemented it using Node.

## Usage

```bash
npm install comics-feed
comics-feed [.rss|url]
```

## Tested on

http://feed.dilbert.com/dilbert/daily_strip  
http://feeds.feedburner.com/uclick/dilbert-classics

## TODO

- Error handling
  - invalid URL
  - malformed feed
  - scrape error

## SAAS on Heroku

[heroku-comics-scraper](leesei/heroku-comics-feed) uses this module to provide a subscrible RSS service.
