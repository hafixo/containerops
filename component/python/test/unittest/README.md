## Python unittest Docker Component

### What's the Component?
The [unittest](https://docs.python.org/3/library/unittest.html) unit testing framework was originally inspired by JUnit and has a similar flavor as major unit testing frameworks in other languages.

### Learn how to build it?
Use the `docker build` command build the image
```bash
docker build -t containerops/unittest .
```

### Component Usage
```bash
docker run --rm -e CO_DATA='git-url=https://github.com/minhhh/regex.git entry-path=.' containerops/unittest
docker run --rm -e CO_DATA='git-url=https://github.com/minhhh/regex.git entry-path=. version=python' containerops/unittest
```

### Parameters
- `git-url` is the source git repo url
- `version` is one of `python`, `python2`, `python3`, `py3k`.  default is `py3k`
- `entry-path` is the entry file or path for unittest

### Versions 1.0.0