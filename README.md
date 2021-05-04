# nemo-docs

Documentation for NEMO

## Publishing

To rebuild, just push commits to `master`. Read the Docs will pick them up automatically.

Automatic deploys can be configured [here](https://readthedocs.org/dashboard/nemo/integrations/).

## Development

Local testing (verified on OSX with Python 3.7.6):

1. `pip3 install -r requirements.txt`
1. `make html`
1. `open _build/html/index.html`

More info at [Read the Docs](https://docs.readthedocs.io/en/stable/intro/getting-started-with-sphinx.html) docs.

### Upgrading dependencies

1. Temporarily change `==` to `>=` in requirements.txt
1. `pip3 install -r requirements.txt --upgrade`
1. `pip3 freeze > requirements.txt`

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
