# word-count

Demonstrates searching for a file in plain python, with rust singlethreaded and with rust multithreaded. 

## Build

```shell
python setup.py install
```

## Usage

```python
from word_count import search_py, WordCounter

search_py("path/to/file", "word")
WordCounter("path/to/file").search("word")
WordCounter("path/to/file").search_sequential("word")
```

## Benchmark

There is a benchmark in `tests/test_word_count.py`:

```shell
pytest -v tests
```