# flake8-todos

Plugin for [flake8](http://flake8.pycqa.org/en/latest/) linter to check TODOs in the project.


Good:

```python
# TODO(gram): check performance
# https://github.com/eclecticiq/flake8-todos/issues/1337
```

Bad:

```python
# FIXME idk how it works lol
```

Checks:

+ **T001**: use TODO instead of FIXME (or BUG) for consistency.
+ **T002**: add author into TODO ([motivation](https://dave.cheney.net/practical-go/presentations/qcon-china.html#_dont_comment_bad_code_rewrite_it)).
+ **T003**: add link on issue into TODO.
+ **T004**: missed colon in TODO.
+ **T005**: missed text in TODO.
+ **T006**: write TODO instead of ToDo (use upper case).

## Installation

```bash
python3 -m pip install --user flake8-todos
```

## Usage

Check that plugin was added in your flake8:

```bash
$ python3 -m flake8 --version
3.7.7 (flake8-todos: 1.0.0, mccabe: 0.6.1, pycodestyle: 2.5.0, pyflakes: 2.1.1) CPython 3.6.7 on Linux
```

If you don't see `flake8-todos` in the previous command output, check that `flake8` and `flake8-todos` is installed in the same interpreter.

If everything is OK, run `flake8`:

```bash
python -m flake8 example.py
```

## License

The content of this repository is released under the [3-clause BSD license](http://opensource.org/licenses/BSD-3-Clause).
See the [LICENSE](LICENSE) file for more information.
