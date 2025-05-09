[![Build Status](https://github.com/dart-lang/tools/actions/workflows/html.yaml/badge.svg)](https://github.com/dart-lang/tools/actions/workflows/html.yaml)
[![pub package](https://img.shields.io/pub/v/html.svg)](https://pub.dev/packages/html)
[![package publisher](https://img.shields.io/pub/publisher/html.svg)](https://pub.dev/packages/html/publisher)

A Dart implementation of an HTML5 parser.

## Usage

Parsing HTML is easy!

```dart
import 'package:html/parser.dart';

void main() {
  var document = parse(
      '<body>Hello world! <a href="www.html5rocks.com">HTML5 rocks!');
  print(document.outerHtml);
}
```

You can pass a String or list of bytes to `parse`. There's also `parseFragment`
for parsing a document fragment, and `HtmlParser` if you want more low level
control.

## Background

This package was a port of the Python
[html5lib](https://github.com/html5lib/html5lib-python) library.
