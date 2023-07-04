# Web Scraping
### videos/resources
  - [login and scrape data w/ playwright and python](https://www.youtube.com/watch?v=H2-5ecFwHHQ&t=60s)
  - [playwright tutorial](https://www.youtube.com/watch?v=yp1o9biMMWU)
  - [xpath cheatsheet](https://devhints.io/xpath)
## What are the key differences between scraping static and dynamic websites?
  Scraping static websites are fixed HTML files and dynamic websites are generated with JS, AJAX, and server-side scripting and can change dynamically

## Explain at least three techniques or best practices that can be employed to avoid getting blocked while scraping websites.
- respect the Robots.txt
- Do not follow the same crawling pattern
- Make crawling slower and do not slam the server or go ahead and rm -rf around and find out- AKA BLOCKED

## What is Playwright, and how does it assist in web scraping tasks? Provide an example of a use case where Playwright would be particularly beneficial.

    Playwright is an open-source library developed by Microsoft that provides a high-level API for automating web browsers. It supports multiple browsers such as Chrome, Firefox, and    WebKit, and allows you to automate browser actions, interact with web pages, and extract data. Playwright can be used for various purposes, including web scraping.

    Consider a scenario where you want to scrape data from a dynamic website that heavily relies on JavaScript to load content. Traditional scraping techniques may not be effective in     retrieving the complete and up-to-date data. In such cases, Playwright can assist by providing a headless browser environment that executes JavaScript and allows you to interact     with the website as if you were using a real browser.

    With Playwright, you can navigate to the target website, perform user interactions (such as clicking buttons, filling forms, or scrolling), wait for certain elements to load, and    extract the desired data from the resulting page. Playwright's powerful API allows you to automate these tasks easily.

## Describe the purpose of using Xpath in web scraping, and provide an example of an Xpath expression to select a specific HTML element from a webpage.
    XPath (XML Path Language) is a query language used to navigate and select elements within an XML or HTML document. It is commonly used in web scraping to locate specific elements or extract data from web pages. XPath provides a concise and powerful way to traverse the document's structure and identify elements based on their attributes, tags, or hierarchical relationships.
  The following example shows xpath grabbing H1 elements:
  `//div[@class='container']/h1`

## things i want to know more about
  automation scraping that alters crawling behavior and making requests through proxies