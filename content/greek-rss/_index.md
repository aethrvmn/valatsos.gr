---
type: "page"
showTableOfContents: true
---

# Greek News RSS Feed Generator

This project serves to promote reading news from Greek news sources using RSS. 
Unfortunately most Greek news media don't provide an RSS feed, probably in order to promote their paid newsletters. In any case, newsletters serve only to spam the inbox, and so a solution is needed.

## Media List

So far I generate RSS feeds for the following outlets:

- ### [liberal.gr](liberal-gr/) (Market Liberals)


## Origin

The idea of this project was inspired by [this repository](https://github.com/capjamesg/openai-blog-rss). Credits to the original author for laying the groundwork.

## How It Works

This generator extracts articles from different categories of the selected news website. After curating the content and removing ads and non-essential components, it produces an RSS feed for each category.

### Hosting and Updates

The RSS feeds are hosted on my personal website, and I've set up a cronjob to refresh the XML files every hour. You can subscribe to them to get the latest content directly to your favorite RSS reader.

### Future Goals

The goal is to expand this tool to other Greek media outlets.

## Contributions

Feel free to contribute! If you're familiar with the structure of other media outlets, your expertise can help expand the reach of this tool.
