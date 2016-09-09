# Processing.py and Arduino

Presentation at [Pyunconf](http://pyunconf.de/), Sat 10, 2016

## Build the presentation

This presentation was built with Markdown, [Pandoc](http://pandoc.org/MANUAL.html#producing-slide-shows-with-pandoc) and [Reveal.js](http://lab.hakim.se/reveal-js/#/).

To build it yourself, install Reveal.js via `bower`

```bash
bower install reveal.js
```

Then type

```bash
pandoc -t revealjs -s main.md -o main.html -V revealjs-url=./bower_components/reveal.js -V theme=sky
```

Open `main.html` in Google Chrome or Chromium.

## License

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons Lizenzvertrag" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />Dieses Werk ist lizenziert unter einer <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Namensnennung 4.0 International Lizenz</a>.
