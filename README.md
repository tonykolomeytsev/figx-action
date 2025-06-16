# Figx GitHub Action

Run the [`figx`](https://github.com/tonykolomeytsev/figx) CLI tool in GitHub Actions.

## Usage

```yaml
jobs:
  figx:
    runs-on: ubuntu-latest
    steps:
      - uses: tonykolomeytsev/figx-action@v0.6
        with:
          command: import
          args: //ui/kit/...
          token: ${{ secrets.FIGMA_PERSONAL_TOKEN }}
```

| Name    | Description                    | Required |
| ------- | ------------------------------ | -------- |
| `command` | Command to run (e.g. `import`) | ✅ Yes    |
| `args`    | Arguments for the command      | ✅ No     |
| `token`   | Figma token if needed          | ❌ No     |
