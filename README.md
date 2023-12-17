<p align="center">
<p align="center">
   <img width="25%" height="20%" src="https://raw.githubusercontent.com/Florents-Tselai/cookiecutter-postgres-extension/main/docs/img/DALL·E%202023-12-17%2019.55.35%20-%20An%20elephant%20sitting%20comfortably%2C%20holding%20a%20python%20gently%20in%20its%20lap.%20The%20elephant%2C%20with%20a%20caring%20expression%2C%20is%20feeding%20cookies%20to%20the%20python.%20The%20sce.png" alt="Logo">
  </p>
  <h1 align="center">cookiecutter-postgres-extension</h1>
  <p align="center">
  <strong>The missing cookiecutter for a Postgres extension</strong>
    <br> <br />
    <a href="#features"><strong> Features</strong></a> |
    <a href="#installation"><strong> Installation </strong></a> |
    <a href="#usage"><strong> Usage </strong></a>
   </p>
<p align="center">

## Features

The missing cookiecutter for a Postgres extension

* Pre-populated extension files (`Makefile,` `.control,` `,c`, `.h`, `.sql`) with stubs.
* Regression Tests
* Out-of-the-box GitHub Actions for building on multiple Postgres versions
* Docker support
* [pgxn](https://pgxn.org) integration

## Installation

You'll need to have [cookiecutter](https://cookiecutter.readthedocs.io/) installed.

    pip install cookiecutter
    or
    python3 -m pip install cookiecutter
    

## Usage

Run `cookiecutter gh:Florents-Tselai/cookiecutter-postgres-extension` and then 
answer the prompts.

The prompt answers will be used to populate the [standard Postgres 
extension files](https://www.postgresql.org/docs/current/extend-extensions.html#EXTEND-EXTENSIONS-FILES)
