[pre-commit](https://pre-commit.com) hook to invoke
[Pyright](https://github.com/Microsoft/pyright), but executed through
[Poetry](https://python-poetry.org) so that pyright uses the correct Python
environment.

This hook does not set up pyright for you! You can either use
[this wrapper](https://pypi.org/project/pyright) by installing it as a dev
dependency in poetry, or require that all developers have pyright installed
on their systems through some other means.

To use this hook:
```
- repo: https://github.com/wlritchi/pre-commit-poetry-pyright
  rev: '1.0.0'
  hooks:
  - id: poetry-pyright
```
