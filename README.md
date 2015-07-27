# python-semantic-release [![Build status][build-badge]][last-build] [![Coverage status][coverage-badge]][last-build]

Automatic semantic versioning for python projects

> **This is not usable, yet.**

## Install
```
pip install semantic-release
```

## Usage
The general idea is to have some sort of tag in commit messages that indicates certain types of changes.
If a commit message lack a tag it is ignored. Running release can be run locally or from a CI service.

Creating a new release: `$ semantic-release new`

### Configuration
All configuration described here belongs in `setup.cfg` in a section: `semantic-release`.

#### Tags
There are a set of tags used to evaluate the changes from commit messages. They can be configured
to meet what you want them to be. The different tags are listed below with their defaults.

* **Major change:** `:boom:` :boom:
* **Minor change:** `:sparkles:` :sparkles:
* **Patch change:** `:bug:` :bug:
* **Upgrade dependency:** `:arrow_up:` :arrow_up: (will trigger minor version change)


[build-badge]: https://ci.frigg.io/relekang/python-semantic-release.svg
[coverage-badge]: https://ci.frigg.io/relekang/python-semantic-release/coverage.svg
[last-build]: https://ci.frigg.io/relekang/python-semantic-release/last/