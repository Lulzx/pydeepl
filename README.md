# pydeepl
An API wrapper for deepl.com translating service.

## Installation

```python
pip install pydeepl
```

## Getting Started

### Python Version

Pydeepl was written for both python 2 and python 3.

### Add Pydeepl to your application

```python
import pydeepl

sentence = 'I like turtles.'
from_language = 'EN'
to_language = 'ES'

translation = pydeepl.translate(sentence, to_language, from_lang=from_language)
print(translation)

# Using auto-detection
translation = pydeepl.translate(sentence, to_language)
print(translation)
```

## Supported Languages

Pydeepl supports these languages:

| Code | Language      |
|------|---------------|
| auto | _Auto detect_ |
| DE   | German        |
| EN   | English       |
| FR   | French        |
| ES   | Spanish       |
| IT   | Italian       |
| NL   | Dutch         |
| PL   | Polish        |

> Note that auto detection only is possible for the source language.

## Disclaimer

DeepL is a product from DeepL GmbH. More info: [deepl.com/publisher.html](https://www.deepl.com/publisher.html)

This package has been heavily inspired by [node-deepls](https://github.com/chriskonnertz/DeepLy) and [node-deepls](https://github.com/pbrln/node-deepl).

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details
