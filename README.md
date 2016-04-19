# markdown-it-named-headings
 
> Add IDs to heading elements in markdown-it

A plugin for [markdown-it][] to add `id` attributes to *h1...h6* elements.

```js
md.render('# Example Header') 
=> '<h1 id="example-header">Example</h1>'
```

[![Status](https://travis-ci.org/rstacruz/markdown-it-named-headings.svg?branch=master)](https://travis-ci.org/rstacruz/markdown-it-named-headings "See test builds")

## Install

```
npm install --save markdown-it-named-headings
```

## Usage

```js
var md = require('markdown-it')()
  .use(require('markdown-it-named-headings'))

md.render('# hello')
```

[markdown-it]: https://github.com/markdown-it/markdown-it
[markdown-it-named-headers]: https://www.npmjs.com/package/markdown-it-named-headers

## Prior art

This works exactly like [markdown-it-named-headers][], except this plugin operates on the token level, not the renderer. The result is that it can be chained with other markdown-it plugins that would want to have access to the ID.

## Thanks

**markdown-it-named-headings** © 2016+, Rico Sta. Cruz. Released under the [MIT] License.<br>
Authored and maintained by Rico Sta. Cruz with help from contributors ([list][contributors]).

> [ricostacruz.com](http://ricostacruz.com) &nbsp;&middot;&nbsp;
> GitHub [@rstacruz](https://github.com/rstacruz) &nbsp;&middot;&nbsp;
> Twitter [@rstacruz](https://twitter.com/rstacruz)

[MIT]: http://mit-license.org/
[contributors]: http://github.com/rstacruz/markdown-it-named-headings/contributors
