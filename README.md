# action-setup-artemis

A GitHub Action to setup [Artemis](https://github.com/toitware/artemis-releases).

## Basic usage

See [action.yml](action.yml) for a complete list of options and outputs.

```yaml
steps:
- uses: actions/checkout@v4

- uses: toitware/action-setup-artemis@v1.1.0
  with:
    version: 'v0.15.3'

- run: artemis --version
```

If no `version` is specified, the latest version is used.
