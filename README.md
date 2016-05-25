# bump-version

`bump-version` is a convenience utility for updating the version in a
gradle project using [git flow](http://nvie.com/posts/a-successful-git-branching-model/).

## Installation

- install [git-flow](https://github.com/nvie/gitflow) tools
- copy `bump-version` to `bin/` directory of your project
- create or update `gradle.properties` file to have a version property:

```groovy
version = 0.0.1
```

## Using

Follow the git flow work flow to create a release branch, then:

```bash
bin/bump-version 1.2.3
```

where (1.2.3 is the version of the release)


## TODO
- add support for non-gradle projects. This should be simple: look for
gradle.properties first and then a file called VERSION. It may require
updating the regex to allow the version file to not have the "version =" part.
