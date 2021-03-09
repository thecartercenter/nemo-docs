# nemo-docs

Documentation for NEMO

## Publishing

To rebuild, just push commits to `master`. Read the Docs will pick them up automatically.

Automatic deploys can be configured [here](https://readthedocs.org/dashboard/elmo-nemo/integrations/).

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
