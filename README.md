# Mass Anna's Archive downloader

Python tool for turning a list of work titles into downloads from Anna's Archive.

Base Selenium code from https://github.com/Nquxii/anna-dl

# Usage

To get requirements:
`pip install -r requirements.txt`

then

`python dl.py`

## Features

- Automatically downloads titles in a .txt file into location of choice
- Proceeds with other titles if one download fails
- Configurations available in `config.json`:
  - `destination`: Absolute location for downloads; default `/titles`
  - `source`: Relative location for .txt file; default `booklist.txt`
  - `language`: Language to filter by; default `English`
  - `fileType`: Filetype to filter for; default `EPUB`; options include any valid Anna's Archive type, such as `MOBI`, `PDF`, `html`
  - `count`: Number of search results to check for LibGen links; default is `3`. Keep in mind that not every title may have a LibGen link within this number of results, or even at all.

## Format for `booklist.txt`

Norwegian Wood

or

Norwegian Wood, Haruki Murakami

or

murakami norwegian wood

Each line is one search term.
