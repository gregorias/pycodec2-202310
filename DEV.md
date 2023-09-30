# pycodec-202310 — DEV

This file is meant for developers. It provides instruction on how to
work with the repository.

## Dev Environment Setup

Install lefthook:

    lefthook install

Install Pipenv:

    pipenv install --dev

## ADRs

This project uses Pipenv to simplify managing development environment
dependencies. It does not use Poetry, because Poetry does not sure building
impure Python wheels (those with Cython), so it would be quite surprising to
have Poetry AND use setuptools directly to build this package.
