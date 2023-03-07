# NEMO docs

Documentation for [NEMO](https://github.com/thecartercenter/nemo/).

## Publishing

To rebuild, just push commits to `main`. Read the Docs will pick them up automatically.

Automatic deploys can be configured [here](https://readthedocs.org/dashboard/getnemo/integrations/).

## Development

Local testing (on Apple Silicon with Python 3.8.X):
As of 2/24/23, I couldn't get the pandas package to compile with Apple silicon, so defaulted to using the virtual arch x86 environment.

1. `arch -x86_64 zsh`
1. run `arch` command to confirm you are now running i386
1. `pip3 install pandas` to confirm it installs
1. `pip3 install -r requirements.txt`
1. `make html` (note you may have to add Python3.8 to your path for this to work)

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
