# Contributing to pyaww

First, thanks for taking the time to consider contributing! ❤️ All contributions are welcomed and encouraged.

## Contributing

1. [Create an issue and assign it to yourself](https://github.com/ammarsys/pyaww/issues).
2. Fork the repository.
3. Locally clone your fork,

```
git clone https://github.com/yourname/pyaww
cd pyaww
```

4. Commit your changes, 

```
git add pyaww/x.py
git commit -m "[feat] add support for y in method z"
```

5. Create/update the tests if needed (look at `tests/README.md`), commit them as well,

```
git add tests/test_x.py
git commit -m "[test] create test for parameter y in method z"
```

Please look at the [following](https://gist.github.com/qoomon/5dfcdf8eec66a051ecd85625518cfd13) git guide for commits.

5. Push your changes via `git push -u origin branch`.
6. [Create a PR](https://github.com/ammarsys/pyaww/issues/pulls),
with a good description on the changes you've made.

## General Guidelines

- Follow the `PEP8` rules.
- Use [Google-style](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html) docstrings.
- You must format your code using [black](https://pypi.org/project/black/).
- You must sort imports using [isort](https://pypi.org/project/isort/).
- You must run tests using [pytest](https://pypi.org/project/pytest/) before creating a pull request.
- Your code must be typehinted. Look into `pyright` or `pylance` type checkers if you do not have one.
- Write clean and efficient code.
- Create/update tests.

## How to run the tests?

1. Install the `pytest`, `pytest-asyncio` and the `python-dotenv` library.
2. Navigate to `pyaww/tests/assets` and create `.env`. It should contain:
```dotenv
USERNAME=USERNAME
AUTH=TOKEN
STARTED_CONSOLE=ID
```

To properly test the module, use a "fresh account". Just create an alternative account, make & start a console and 
you're good to go!

3. Ensure your CWD is `pyaww` and not `pyaww/tests` or similar.
4. Run `py -m pytest -s`.
5. Fix if anything is wrong, if not, your tests are fine.
