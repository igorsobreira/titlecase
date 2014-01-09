# titlecase

Titlecase is a port of [Python's titlecase module](https://pypi.python.org/pypi/titlecase/) in Go.

It capitalizes all words in the string to Title Caps attempting to be smart about
small words like a/an/the.

These small words will also be uncapitalized, so titlecase also works with uppercase
strings.

The list of small words which are not capped comes from the New York Times Manual of
Style, plus 'vs' and 'v'.

## Usage:

```go
import "github.com/igorsobreira/titlecase"

func main() {
    println(titlecase.Title("this and that")) // output: "This and That"
}
```

See the tests for all the use cases handled.

Thanks to Stuart Colville for the [Python version](https://pypi.python.org/pypi/titlecase).
And John Gruber for the [original version in Perl](http://daringfireball.net/2008/05/title_case)

## License

```
The MIT License (MIT)

Copyright (c) 2014 Igor Sobreira <igor@igorsobreira.com>

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
```
