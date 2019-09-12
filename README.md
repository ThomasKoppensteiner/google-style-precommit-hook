A handy [pre-commit](http://pre-commit.com/) hook which will run Google's [java
code style formatter](https://github.com/google/google-java-format) [v1.7](https://github.com/google/google-java-format/releases/tag/google-java-format-1.7) for you on your code!

Usage:

```
repos:
- repo: https://github.com/ThomasKoppensteiner/google-style-precommit-hook/
  rev: v1.0.0
  hooks:
    - id: google-style-java
```

*Note*: this file stores Google's code style formatter jar in a `.cache/`
directory so that it doesn't need to be re-downloaded each time.  You will
probably want to add `.cache/` to the `.gitignore` file of the project which
uses this hook.
