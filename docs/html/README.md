# HTML

Zero doesn't just serve HTML as is. URLs to scripts, styles, media, and other HTML files are extracted and compiled. The references are rewritten in the HTML so that they link to the correct output files. All filenames should be relative to the current HTML file.

Zero's HTML bundler is powered by [Parcel](https://parceljs.org/).

**Note:** When linking to other HTML pages, do not put `.html` at the end ie. Use `<a href="/about">` instead of `<a href="/about.html">`. This tells underlying Parcel builder to _code split_ correctly and not bundle `about.html` with this page.
