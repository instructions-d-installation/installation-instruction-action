<div align="center">

# `installation-instruction-action`

**Github action for installing things to your runner with installation instruction config file.**

</div>

## Usage

```yaml
    steps:
      - name: Install from Config File
        uses: instructions-d-installation/installation-instruction-action@0.1.0
        with:
          path: <url to git repo or path to directory or config file>
          options: <options for installation>
```
