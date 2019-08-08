# Scraping Garden Party

August 9, 2019
Geoff Ford
https://geoffford.nz
https://github.com/polsci/

This repo is a website that contains stories from The Garden Party: and Other Stories by Katherine Mansfield. It was built by Geoff Ford as a simple website for students to work with for a web scraping exercise.

It is based on [this text file](/scraping-garden-party/1429-0.txt) from [Project Gutenberg](https://www.gutenberg.org/ebooks/1429).

## The scraping exercise

The scraping task is intended to get students inspecting HTML markup on a very small and simple website and to think about how to write code to extract and follow links and extract specific text.

The scraping task required students to retrieve the 15 links to short stories using CSS selectors and Python and the Requests and BeautifulSoup libraries. They then needed to write some code that looped through the links, built a full URL, retrieved each short story page and output a specific part of the short story page (specifically the text in the paragraph with class="introductory-section"). They were required to put in a 2 second delay between each request using time.sleep().
