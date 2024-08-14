# Scraping Garden Party

Geoff Ford  
https://geoffford.nz/  

## Introduction

This repo contains files for a small and simple Github pages website (i.e. using Jekyll): https://ucdh.github.io/scraping-garden-party/

The site contains stories from The Garden Party: and Other Stories by Katherine Mansfield. It was built by Geoff Ford as a simple website for students to work with for a web scraping exercise.

It is based on [this text file](/scraping-garden-party/1429-0.txt) from [Project Gutenberg](https://www.gutenberg.org/ebooks/1429).

## The scraping exercise

The scraping task is intended to get students inspecting HTML markup on a very small and simple website and to think about how to write code to extract and follow links and extract specific text.

The scraping task required students to retrieve the 15 links to short stories using CSS selectors and Python and the Requests and BeautifulSoup libraries. They then needed to write some code that looped through the links, built a full URL, retrieved each short story page and output a specific part of the short story page (specifically the text in the paragraph with class="introductory-section"). They were required to put in a 2 second delay between each request using time.sleep().

I've added a couple of things subsequently:
* A input field in the left column - you can enter CSS selectors and it will highlight the relevant content. This has been added as a tool to demonstrate CSS selectors in class and for students to try this outside of class.    
* Author and date in HTML metadata and in the page to demonstrate that this could be scraped with text to structure our data. Dates are the dates stories were first published in periodicals from a quick read of Wikipedia OR are 1922-01-01 (the year the collection was first published). Note: only year is displayed on short story pages.  
* A [link](https://ucdh.github.io/scraping-garden-party/to-lhb.html) to one of Mansfield's poems, however in this page the text is loaded via AJAX. This is used to demonstrate that not all text is straightforwardly in the HTML in modern websites.  

## Scraping Garden Party Corpus

A corpus of _Garden Party_ short stories is included in the directory [garden-party-corpus](https://github.com/ucdh/scraping-garden-party/tree/master/garden-party-corpus). You can download a [zip file of the Scraping Garden Party Corpus](https://github.com/ucdh/scraping-garden-party/raw/master/garden-party-corpus.zip). The filenames contain a recognisable version of the short story name. The text files contain the short story without the title.
