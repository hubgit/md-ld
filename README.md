# Markdown-LD

Markdown-LD extends Markdown's [reference link](http://spec.commonmark.org/0.18/#reference-link) syntax to allow easy authoring of structured data.

See [a Markdown-LD example](https://raw.githubusercontent.com/hubgit/markdown-ld/master/example.md) and the equivalent [JSON-LD](https://raw.githubusercontent.com/hubgit/markdown-ld/master/example.json) or [Turtle](https://raw.githubusercontent.com/hubgit/markdown-ld/master/example.ttl).

## The Rules of Markdown-LD

1. References are identifiers in square brackets (`[example]`).
1. Object definitions start with an identifier in square brackets followed by a colon, on a new line with no indentation (`[example]:`)
1. Properties are each on a new line, indented.
1. Values are on a new line, indented twice. Any property can have multiple values.
1. Nested objects are not allowed.
1. Newlines must be escaped (`\n`).
1. Empty lines should be ignored.
1. Markdown-LD files use UTF-8 encoding.

## Differences from existing formats

* Unlike YAML and JSON, there’s no need to use special array markup to distinguish between single and multiple values (in Markdown-LD, all properties should have singular names).
* Unlike Turtle, there’s no need to use angle brackets or quotes.
* Unlike Markdown, the definition has more structure than a URL and a title.
* Unlike JSON, indentation is significant.
* Unlike JSON-LD, there’s no need to use special `@` syntax.
* Unlike microdata, the data does not have to be embedded in HTML.
* Unlike HTML’s `<dl>`, `<dt>` and `<dd>`, there’s a direct mapping between item name and definition.
* Unlike other formats, the format of all “text” values is Markdown.

## Notes

The `type` property of each object is a URL that defines the type of that object in a known schema (e.g. [schema.org](http://schema.org/)).

Data typing of property values is implicit: if the schema is well defined, the type of each value should be derived from the schema.

Markdown-LD is not backwards-compatible with existing Markdown parsers - suggestions to make it so would be appreciated.
