# bluelabs-circleci-orbs

For usage information and latest version, see:

<https://circleci.com/orbs/registry/orb/bluelabs/quality>

## Publishing

CircleCI automatically publishes dev builds to `bluelabs/quality@dev:<branch>`

To promote a dev:master release to prod, you can use:

```
circleci orb publish promote bluelabs/quality@dev:master patch
```

Replace patch with major or minor to control the version field that circleci bumps.

## Manual validation and publishing

```sh
circleci orb validate src/quality.yml
circleci orb publish src/quality.yml bluelabs/quality@dev:latest
```

