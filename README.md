# About

This is a simple tool based on [website-scraper](https://github.com/website-scraper/node-website-scraper) and [website-scraper-puppeteer](https://github.com/website-scraper/website-scraper-puppeteer) projects (and, in turn Headless Chrome / [puppeteer](https://github.com/puppeteer/puppeteer)) that, given a URL of a website, will crawl and download its structure as a set of HTML files, then produce a single ZIP archive, suitable for importing into [Smartcat](https://smartcat.com/) platform for content translation and calculating the translation volume/statistics.

# Disclaimer / License

This is an experimental tool that is provided with no guarantees or obligations. See [MIT-LICENSE.txt](MIT-LICENSE.txt) for more information.


# Installation

Install Node.js as per official instructions:
https://nodejs.org/en/download/

Then run the following command in the current directory to install required modules:

```sh
npm install
```

# Usage

```sh
node download-website <URL>
```

This will create a ZIP archive with the name that follows the `<URL>-<DATETIME>.zip` pattern.

## Uploading to Smartcat

Create a new project in Smartcat and drop the resulting ZIP file onto the first screen of the project creation wizard. This will upload and unpack the contents of the ZIP file. Then proceed with setting up your project as usual.

Remember that processing ZIP files with many files will take some time both at project creation time, at text parsing/indexing and at statistics calculation time.

# Support

Please contact Smartcat team at support@smartcat.com if you have questions on using the tool or our platform, or if you have specific needs with localizing your web site, CMS or a software product.