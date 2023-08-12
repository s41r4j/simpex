# [ 'simpex' -> "simple regex" ]


`simpex` is a python library that simplifies the process of using regular expressions (`regex`). It provides both custom and built-in methods to generate regex patterns, making it easier for developers to match and manipulate text data. Whether you're working with emails, URLs, phone numbers, or other patterns, `simpex` has you covered.

#### _Features_:
- Simplify regex usage in Python.
- Generate regex patterns effortlessly.
- Access external APIs for regex generation.
- Choose from custom or built-in patterns.

<br>

## Installation | [wiki](../../wiki/Getting-Started#installation)

To install `simpex`, use the following command:

```bash
pip install simpex
```

<br>

## Usage | [wiki](../../wiki/Getting-Started#usage)

There are three steps between you and regex pattern you want! Follow below instatructions as _quick guide_, please chak out _[wiki]()_ for comprehensive usage with examples.  

### [step 1]: Importing
- Use the following import statement:
```python
from simpex.simpex import simpex
```

### [step 2]: Creating Object
- `simpex` is a class, so we need to __create an object__ with required parametric data
```python
email = simpex(['test@mail.com', 'admin@email.com', 'example@mail.co'])
```
- check [wiki](), for all available parameters

### [step 3]: Calling Method
- Call your desired method from `custom`, `build-in` or `api-based` to get regex pattern
```
pattern = email.regex() # calling custom method
```
- check [wiki](), for all avaliable methods

<br>


### Contributing

Contributions are welcome! Please follow the guidelines in [CONTRIBUTING.md](CONTRIBUTING.md) to contribute to the project.

### License

This project is licensed under the [MIT License](LICENSE).
