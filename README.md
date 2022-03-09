# Documentation for Rucio

[![Update
Documentation](https://github.com/rucio/documentation/actions/workflows/update_documentation.yml/badge.svg)](https://github.com/rucio/documentation/actions/workflows/update_documentation.yml)
[![Check external
links](https://github.com/rucio/documentation/actions/workflows/check_external_links.yaml/badge.svg)](https://github.com/rucio/documentation/actions/workflows/check_external_links.yaml)

This project contains the documentation for the [rucio](https://github.com/rucio/rucio)
project.

## Documentation Structure

There are two types of documentation hosted for Rucio. Should you wish to
contribute improvements to any of them, follow the guidelines below.

### Markdown documentation

The source for this section lives in the ``docs`` folder within the main branch
of the this GitHub repository. Improvements may be suggested by submitting an
issue or pull request to the **main** branch of the repository.  Once the
changes are approved, GitHub Actions will trigger the build process and publish
on to GitHub pages.

### API Documentation

The source for this section lives in the
[``rucio/rucio``](https://github.com/rucio/rucio/) GitHub repository. There are
two sub-categories that we document:

- [__Rest
  API__](https://github.com/rucio/rucio/tree/master/lib/rucio/web/rest/flaskapi/v1)
- [__Client API__](https://github.com/rucio/rucio/tree/master/lib/rucio/client)

Since the documentation is directly derived from the source, any change to the
documentation needs to be made in the source code.  Please submit an issue or
pull request to the [``rucio/rucio``](https://github.com/rucio/rucio/)
repository with your suggestions for contribution.  Once the changes have been
approved & pushed into the main branch, the changes will be available at
<https://rucio.cern.ch/documentation> on the next day.

## Project Structure

There are 2 branches in this repository:

- main: Containing the build files for Docusaurus
- gh-pages: Hosting the website available at
  [https://rucio.cern.ch/documentation](https://rucio.cern.ch/documentation)

## Git Hooks

The `pre-commit` python package is configured for this repository. The
pre-commit hook checks the syntax and format of the files before commiting. This
saves time in the development process, since minor errors are noticed early.

To install the package and activate the hooks for the project:

```bash
pip install pre-commit
pre-commit install
```
