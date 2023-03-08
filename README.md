This project was bootstrapped with [eask/cli](https://github.com/emacs-eask/cli).

## How to use?

1. Write and design your package in `your-package.el`
2. Install package dependences if any:

  ```sh
  eask install-deps
  ```

3. Prepare for installation, package it: (it will create package to `dist` folder)

  ```sh
  eask package
  ```

4. Install the built package:

  ```sh
  eask install
  ```

## Compile

You would want to compile your elisp file to check if there are errors:

```sh
eask compile
```

## Lint

Linting is often optional but recommended to all elisp developers.

with `checkodc`:

```sh
eask lint checkodc
```

with `package-lint`:

```sh
eask lint package  # for pacakge-lint
```

For more options, see `eask lint --help`!

## Continuous Integration

### CircleCI

```sh
eask generate workflow circle-ci
```

### GitHub Actions

```sh
eask generate workflow github
```

### GitLab Runner

```sh
eask generate workflow gitlab
```

### Travis CI

```sh
eask generate workflow travis-ci
```

For more options, see `eask generate workflow --help`!

## Learn More

To learn Eask, check out the [Eask documentation](https://github.com/emacs-eask).
