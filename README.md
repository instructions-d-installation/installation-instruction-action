<div align="center">

# `installation-instruction-action`

**Github action for installing things to your runner with installation instruction config file.**

</div>

## Usage

```yaml
    steps:
      - name: Install from Config File
        uses: instructions-d-installation/installation-instruction-action@0.1.2
        with:
          path: <url to git repo or path to directory or config file>
          options: <options for installation (optional)>
          version: <installation-instruction version (optional)>
```

### Input

* `path`: Path to directory, file or a remote git repository url containing the config file.
* `options`: Options as string to pass to ibi cli. (Please check locally if it works.)
* `version`: Version of installation-instruction to use. If empty, uses the latest version.


### Example

```yaml
    steps:
      - name: Install from Config File
        uses: instructions-d-installation/installation-instruction-action@0.1.2
        with:
          path: ./install.cfg
          options: --something
```
