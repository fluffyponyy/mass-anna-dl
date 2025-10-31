# Mass Anna's Archive downloader
Python tool for turning a list of work titles into downloads.
Base Selenium code from https://github.com/Nquxii/anna-dl

# Usage
`python dl.py`

## Features
- Automatically downloads titles in a .txt file into location of choice
- Proceeds with other titles if one download fails
- Configurations available in `config.json`:
  - `destination`: Absolute location for downloads; default `/titles`
  - `source`: Relative location for .txt file; default `booklist.txt`
  - `language`: Language to filter by; default `English`
  - `fileType`: Filetype to filter for; default `EPUB`; options include any valid Anna's Archive type, such as `MOBI`, `PDF`, `html`

## Format for `booklist.txt`
Norwegian Wood

or

Norwegian Wood, Haruki Murakami

or

Norwegian Wood, Murakami

