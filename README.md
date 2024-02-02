# Actions composite for pico projects (sdk)


Github actions for build rasp pico projects with sdk.

## Using

> Check for example repo: [insper-embarcados/infra-test](https://github.com/insper-embarcados/infra-test)

Create a `.github/workflow/build.yml` file:

``` yaml
name: Build and test

on:
  workflow_dispatch:
  push:

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - uses: insper-embarcados/pico-build@v13
```
