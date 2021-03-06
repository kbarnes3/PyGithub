# PyGitHub-ReadOnly

PyGitHub-ReadOnly is a fork of [PyGitHub](https://github.com/PyGithub/PyGithub) that supports creating read-only deploy keys. This functionality is available in pull requests to PyGitHub. See [here](https://github.com/PyGithub/PyGithub/pull/467) and [here](https://github.com/PyGithub/PyGithub/pull/570). Once this functionality is available in versions of PyGitHub available on PyPi, expect this fork to be deprecated.

[![Build Status](https://travis-ci.org/PyGithub/PyGithub.svg?branch=master)](https://travis-ci.org/PyGithub/PyGithub)
[![PyPi](https://img.shields.io/pypi/dm/pygithub.svg)](https://pypi.python.org/pypi?%3Aaction=search&term=pygithub&submit=search)
[![readthedocs](https://img.shields.io/badge/docs-latest-brightgreen.svg?style=flat)](http://pygithub.readthedocs.org/en/stable)
[![License](https://img.shields.io/badge/license-LGPL-blue.svg)](https://en.wikipedia.org/wiki/GNU_Lesser_General_Public_License)

PyGitHub is a Python (2 and 3) library to access the [GitHub API v3].
This library enables you to manage [GitHub] resources such as repositories, user profiles, and organizations in your Python applications.

[GitHub API v3]: https://developer.github.com/v3
[GitHub]: https://github.com

## Simple Demo

```python
from github import Github

# First create a Github instance:
g = Github("user", "password")

# Then play with your Github objects:
for repo in g.get_user().get_repos():
    print repo.name
```

## Documentation

More information can be found on the [PyGitHub documentation site.](http://pygithub.readthedocs.io/en/latest/introduction.html)

## Development

### Contributing

Long-term discussion and bug reports are maintained via GitHub Issues.
Code review is done via GitHub Pull Requests.

For more information read [CONTRIBUTING.md].

[CONTRIBUTING.md]: /CONTRIBUTING.md

### Maintainership

We're actively seeking maintainers that will triage issues and pull requests and cut releases.
If you work on a project that leverages PyGitHub and have a vested interest in keeping the code alive and well, send an email to someone in the MAINTAINERS file.
