## Overview
A simple git tarball CLI for Github repositories and subdirectories.


## Quick Start
- `npm i gitto -g`
- `gitto fetch <github_repo_url>`
- `gitto fetch <github_repo_url> --directory ~/repos`


## Description
The commands above will install `gitto` to your local machine and make the `gitto` command globally available.
You can then download any public Github repository or subdirectory per the quick start instructions.


## How it works
Gitto downloads a copy of the main repository's tarball to your local machine, unzips the file, formats it, and then store the formatted version in your current working directory. Alternatively, you can pass in a `--directory` parameter indicating where you want to install the repository. As part of the formatting, we automatically remove the `.git` directory and the initial download so you'll start with a clean working repository.


## Why we built this
We ran into issues using Degit on some nested directories and felt like their CLI wasn't expansive enough for a couple of use-cases we have in mind.


## Config
Gitto will read the following variables from your gitto config file and use them as your defaults. You can override the location of your config file by passing `-c path/to/config` in any command.
- GITHUB_TOKEN
- DIRECTORY


## Author
- Eric Hubbell
- eric@erichubbell.com


## Inspiration
- degit
- gittar


## Contributions
- Please open an Issue describing the PR you want to submit so we can engage briefly before starting work.