# pbxproj - a language grammar for highlight.js

## Usage

Simply include the Highlight.js library in your webpage or Node app, then load this module.

### Static website or simple usage

Simply load the module after loading Highlight.js.  You'll use the minified version found in the `dist` directory.  This module is just a CDN build of the language, so it will register itself as the Javascript is loaded.

```html
<script type="text/javascript" src="/path/to/highlight.min.js"></script>
<script type="text/javascript" src="/path/to/pbxproj.js"></script>
<script type="text/javascript">
  hljs.highlightAll();
</script>
```


### Using directly from the UNPKG CDN

```html
<script type="text/javascript"
  src="https://unpkg.com/highlightjs-robots-txt@0.9.1/dist/robots-txt.min.js"></script>
```

- More info: <https://unpkg.com>

### With Node or another build system

If you're using Node / Webpack / Rollup / Browserify, etc, simply require the language module, then register it with Highlight.js.

```javascript
var hljs = require('highlight.js');
var hljsPbxproj = require('highlightjs-pbxproj');

hljs.registerLanguage("pbxproj", hljsPbxproj);
hljs.highlightAll();
```

## License

Highlight.js is released under the MIT License. See [LICENSE][1] file
for details.

### Author

Leitmotif GmbH <hello@leitmotif.dev>

### Maintainers

Florian Albrecht
Michael Ehrmann

## Links

- The official site for the Highlight.js library is <https://highlightjs.org/>.
- The Highlight.js GitHub project: <https://github.com/highlightjs/highlight.js>

[1]: https://github.com/leitmotif-dev/highlightjs-pbxproj/blob/master/LICENSE
