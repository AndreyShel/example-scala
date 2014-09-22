Scala <3 [Codecov.io](https://codecov.io)
=======
| [https://codecov.io/][1] | [@codecov][2] | [hello@codecov.io][3] |
| ------------------------ | ------------- | --------------------- |
=======


[![Build Status](https://secure.travis-ci.org/codecov/example-scala.svg?branch=master)](http://travis-ci.org/codecov/example-scala) [![codecov.io](https://codecov.io/github/codecov/example-scala/coverage.svg?branch=master)](https://codecov.io/github/codecov/example-scala)

> This repo is simply an example of how to integrate with Codecov.io for your **awesome** Scala project!



## Usage

```sh
sudo pip install codecov
codecov --token=<repo token>
```

## Require min coverage
```sh
codecov --min-coverage=75
```
> if coverage is under `75` codecov will trigger your build to fail

# [![travis-org](https://avatars2.githubusercontent.com/u/639823?v=2&s=50)](https://travis-ci.org) Travis C
> Append to your `.travis.yml`

```yml
install:
    sudo pip install codecov
after_success:
    codecov
```

> ### Start testing with [Travis](https://travis-ci.org/)

# [![codeship](https://avatars1.githubusercontent.com/u/2988541?v=2&s=50)](https://codeship.io/) Codeship
> Append to your `Test Commands` *after* your test commands

```sh
sudo pip install codecov
codecov --token=<repo token>
```

> ### Start testing with [Codeship](https://codeship.io/)


# [![circleci](https://avatars0.githubusercontent.com/u/1231870?v=2&s=50)](https://circleci.com/) Circle CI
> Append to your `circle.yml` file

```yml
test:
    post:
        - sudo pip install codecov
        - codecov --token=<repo token>
```
> ### Start testing with [Circle CI](https://circleci.com/)




[1]: https://codecov.io/
[2]: https://twitter.com/codecov
[3]: mailto:hello@codecov.io
