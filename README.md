# Scraping Garden Party

This repo is a website that contains stories from The Garden Party: and Other Stories by Katherine Mansfield. It was built by [Geoff Ford](https://geoffford.nz) as a simple website for students to work with for a web scraping exercise.

It is based on [this text file](/scraping-garden-party/1429-0.txt) from [Project Gutenberg](https://www.gutenberg.org/ebooks/1429).

The scraping task requires students to retrieve the 15 links to short stories using CSS selectors and Python and the Requests and BeautifulSoup libraries. They then needed to write some code that looped through the links, built a URL, retrieved each short story page and retrieved a specific part of the short story page. They were required to put in a 2 second delay between each request using time.sleep().
