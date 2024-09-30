# pyLogix

`pyLogix` is a Python library that provides utility functions for text processing and a configurable logging system. It is designed to assist developers with common text manipulation tasks while also providing a robust logging mechanism to track application behavior.

## Features
  
- **Logging Functionality**:
  - Configurable logging levels (DEBUG, INFO, WARNING, ERROR) to track function calls and errors.
  - Output logs to console or a specified log file.

## Installation

You can install the library using `pip`:

```bash
pip install pyLogix
```

## Usage

### Importing the Library

You can import the utility functions and the logger as follows:

```python
from pyLogix.utils import count_words, reverse_text, find_substring
from pyLogix.logger import logger, set_log_level
```

### Setting Log Level

You can configure the logging level at the beginning of your application:

```python
set_log_level('DEBUG')  # Options: DEBUG, INFO, WARNING, ERROR
```

### Example Functions

#### 1. Count Words

This function counts the number of words in a given string.

```python
text = "Hello, this is a sample text for testing."
word_count = count_words(text)
print(f"Word Count: {word_count}")
```

#### 2. Reverse Text

This function reverses a given string.

```python
text = "Hello, World!"
reversed_text = reverse_text(text)
print(f"Reversed Text: {reversed_text}")
```

#### 3. Find Substring

This function checks if a specified substring exists within a given string.

```python
text = "Hello, this is a sample text for testing."
substring = "sample"
exists = find_substring(text, substring)
print(f"Does the substring exist? {exists}")
```

### Logging Example

You can log messages at various levels using the logger:

```python
logger.debug("This is a debug message.")
logger.info("This is an info message.")
logger.warning("This is a warning message.")
logger.error("This is an error message.")
```

## Running Tests

To ensure that the library works as intended, you can run the tests located in the `tests/` directory.

```bash
pytest tests/
```

## Contributing

Contributions are welcome! If you find any bugs or have suggestions for improvements, feel free to submit an issue or a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact

For any inquiries, you can reach me at [prasadchavan1203@gmail.com](mailto:your.email@example.com).
