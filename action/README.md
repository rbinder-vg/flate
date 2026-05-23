# flate GitHub Action

Install the [flate](https://github.com/home-operations/flate) CLI on Linux, macOS, or Windows GitHub runners.

```yaml
steps:
  - uses: home-operations/flate/action@main
    with:
      version: latest
  - run: flate get ks --path ./kubernetes
```

## Inputs

| Name      | Description                                                                     | Default                      |
| --------- | ------------------------------------------------------------------------------- | ---------------------------- |
| `version` | flate version (e.g. `0.1.3`)                                                    | latest release               |
| `bindir`  | Alternative install location                                                    | `$RUNNER_TOOL_CACHE/flate/…` |
| `token`   | GitHub token for `api.github.com` (use to avoid rate limits on `latest` lookup) | none                         |
