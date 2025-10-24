# NEMO docs

Documentation for [NEMO](https://github.com/thecartercenter/nemo/).

## Publishing

To rebuild, just push commits to `main`. Read the Docs will pick them up automatically.

Automatic deploys can be configured [here](https://readthedocs.org/dashboard/getnemo/integrations/).

## Development

### Requirements

1. Python 3 – Check if available in your terminal: `python3 --version` or `pyenv versions`

### Setup

(Last verified on Mac v15 M1).

1. `pip3 install pandas` to confirm it installs
1. `pip3 install -r requirements.txt` to install everything else
1. `make html`
1. `open _build/html/index.html`

More info at [Read the Docs](https://docs.readthedocs.io/en/stable/intro/getting-started-with-sphinx.html) docs.

### Upgrading dependencies

1. Temporarily change `==` to `>=` in `requirements.txt`
1. `pip3 install -r requirements.txt --upgrade`
1. `pip3 freeze > requirements.txt`

Note that the historical https://github.com/sassafrastech/nemo-docs-redirect may also need to be updated.

### Working with translations

Once changes are made to the PO file in Transifex:

Pull changes from Transifex to local repo (replace "fr" with the language code you are translating):

```
tx pull -l fr
```

Then build with this modified command:

```
make -e SPHINXOPTS="-D language='fr'" html
```
