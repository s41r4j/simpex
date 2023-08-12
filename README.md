<h1 align=center>simpex</h1>

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

### 1) Importing
- Use the following import statement:
```python
from simpex.simpex import simpex
```

### 2) Creating Object
- `simpex` is a class, so we need to __create an object__ with required parametric data (check [wiki](), for all available parameters)
```python
# creating an onject named `email`
email = simpex(['test@mail.com', 'admin@email.com', 'example@mail.co'])
```

### 3) Calling Method 
- Call your desired method from `custom`, `build-in` or `api-based` to get regex pattern (check [wiki](), for all avaliable methods)
```python
# calling custom method
pattern = email.regex()
```

> output: `print(pattern)` -> `^[a-z]+\@[a-z]+\.[a-z]*$`


<br><hr>

## License & Contributing
- This is an __open source project__, licensed under the [MIT License](LICENSE).
- __All contributions are welcome!__
  - To contribute to `simpex` project, fork the repository, make your changes, and submit a pull request.
  - Be sure to follow our coding style and include tests for any new functionality.
  - When submitting a pull request, please provide a clear description of your changes.
  - Your contributions help improve the project for everyone.

