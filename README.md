# simpex 
> Simplified Regex for Python

![simpex Logo](path_to_logo_if_available.png)

`simpex` is a Python library that simplifies the process of using regular expressions (`regex`). It provides both custom and built-in methods to generate regex patterns, making it easier for developers to match and manipulate text data. Whether you're working with emails, URLs, phone numbers, or other patterns, `simpex` has you covered.

### Features
- Simplify regex usage in Python.
- Generate regex patterns effortlessly.
- Access external APIs for regex generation.
- Choose from custom or built-in patterns.

### Installation

To install `simpex`, use the following command:

```bash
pip install simpex
```

### Usage

#### Custom Method

Given a sample dataset with a minimum of 2 values, the custom method returns a regex pattern.

```python
import simpex

data_set = ['example@gmail.com',
            'test@yahoo.com',
            'admin@proton.me']

pattern = simpex.generate_pattern(data_set)
```

#### Built-in Method

Use built-in methods to obtain regex patterns. Check all available built-in methods in the [wiki](wiki_link).

```python
import simpex

pattern = simpex.patterns('email')
```

### Available Built-in Patterns

- `email`
- `phone`
- `url`
- `ipv4`
- `ipv6`
- `mac`
- `credit_card`
- `date`
- `hex_color`
- `html_tag`

### API Integration

`simpex` integrates with external APIs to enhance regex pattern generation.

| API  | Endpoint                                  | Required Data Type | Outputs         |
| ---- | ----------------------------------------- | ------------------ | --------------- |
| 0    | information (this only)                   | none / null        | info - str      |
| 1    | [https://saasbase.dev/tools/regex-generator](https://saasbase.dev/tools/regex-generator) | english to regex (ai) - str | single - str   |
| 2    | [https://www.autoregex.xyz](https://www.autoregex.xyz) | english to regex (ai) - str | single - str   |
| 3    | [https://regex.murfasa.com](https://regex.murfasa.com) | english to regex (ai) - str | single - str   |
| 4    | [https://regex.ai](https://regex.ai)       | multiple data set | multiple - list |

### Example

For instance, using the `email` built-in method or the custom method will return the following regex pattern: `^[a-zA-Z0-9]+@[a-zA-Z0-9]+\.[a-zA-Z0-9]*`.

### Contributing

Contributions are welcome! Please follow the guidelines in [CONTRIBUTING.md](CONTRIBUTING.md) to contribute to the project.

### License

This project is licensed under the [MIT License](LICENSE).
