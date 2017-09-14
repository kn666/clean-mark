<h1 align="center">
  ➹ Clean-mark
  <br>
</h1>

<p align="center">
  <a href="https://www.npmjs.com/package/clean-mark"><img src="https://img.shields.io/npm/v/clean-mark.svg" alt="npm version"></a>
  <a href="https://standardjs.com"><img src="https://img.shields.io/badge/code_style-standard-brightgreen.svg" alt="Standard - JavaScript Style Guide"></a>
</p>

Convert an article into a clean Markdown text file.

> ./bin/clean-mark "http://some-website.com/some-fancy-article"

The article will be automatically named using the URL path name.

This project depends on the [A-Extractor](https://github.com/croqaz/a-extractor) project, a database of expressions used for extracting content from blogs and articles.


Tested on all major news sites. On some websites, the text, or links are cut from the article.
In this case, you have to manually edit the resulted text,

AND

raise an [issue on A-Extractor](https://github.com/croqaz/a-extractor/issues) with the link that doesn't work and I'll add it in the database, so that next time, the text will be extracted correctly.

My desired goals are:

1. Good text extraction
1. More useless text is preferred, instead of wrongly cutting from the actual article
1. Extracting media (images, videos, audio) is not that important
1. Extraction speed is not that important


Implementation steps:

1. Downloads the content of a web page
1. Meta-scrape page details (title, author, date, etc)
1. Sanitizes the ugly HTML
1. Minifies the disinfected HTML
1. Converts the result into clean Markdown text


-----

Made by :copyright: :registered: :radio_button:

Released under the [MIT license](https://raw.githubusercontent.com/croqaz/a-extractor/master/LICENSE).
