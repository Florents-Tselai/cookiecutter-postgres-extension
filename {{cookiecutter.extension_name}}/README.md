# {{cookiecutter.extension_name}}: {{cookiecutter.description}}

[![Build Status](https://github.com/{{cookiecutter.github_username}}/{{cookiecutter.github_repo}}/actions/workflows/build.yml/badge.svg)]
(https://github.com/{{cookiecutter.github_username}}/{{cookiecutter.github_repo}}/actions)

{{cookiecutter.extension_name}} is a Postgres extension that {{cookiecutter.description}}

## Installation

    git clone git@github.com:{{cookiecutter.github_username}}/{{cookiecutter.github_repo}}.git
    cd {{cookiecutter.github_repo}}
    make all
    make install
    make installcheck

## Credits

This extension was created using 
[Florents-Tselai/cookiecutter-postgres-extension](https://github.com/Florents-Tselai/cookiecutter-postgres-extension)