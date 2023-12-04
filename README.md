# postgres-extension cookiecutter template

The missing cookiecutter for a Postgres extension 🎉

* Pre-populated extension files (`Makefile,` `.control,` `,c`, `.h`, `.sql`)
* Tests
* Build on multiple Postgres versions with GitHub Actions

## Installation

You'll need to have [cookiecutter](https://cookiecutter.readthedocs.io/) installed. I recommend pipx for this:

    pip install cookiecutter
    or
    python3 -m pip install cookiecutter
    

## Usage

Run `cookiecutter gh:Florents-Tselai/cookiecutter-postgres-extension` and then 
answer the prompts.

The prompt answers will be used to populate the [standard Postgres 
extension files](https://www.postgresql.org/docs/current/extend-extensions.html#EXTEND-EXTENSIONS-FILES)
