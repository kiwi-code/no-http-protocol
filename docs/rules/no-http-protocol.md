# Forbid specifying http(s) protocol in URLs. (no-http-protocol)

Use `//my.server.com` instead.


## Rule Details

This rule aims to...

Examples of **incorrect** code for this rule:

```js

var invalidVar = 'http://my.server.com';
var invalidVar = 'https://my.server.com';
$.get('http://my.site.com');
$.get('https://my.site.com');
let http = 'http://my.site.com';
let https = 'https://my.site.com';

```

Examples of **correct** code for this rule:

```js

var invalidVar = '//my.server.com';
var invalidVar = '//my.server.com';
$.get('//my.site.com');
$.get('//my.site.com');
let http = '//my.site.com';
let https = '//my.site.com';

```

### Options

None

## When Not To Use It

None

## Further Reading

