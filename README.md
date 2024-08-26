# notebook

An ongoing collection of my notes.

## Dependencies

`pip install -U cookiecutter jupyter-book`

## Set Up a New Project

1. `cookiecutter git@github.com:executablebooks/cookiecutter-jupyter-book.git`

2. `cd <book-name>`

3. `python -m venv .venv` 

4. `source .venv/bin/activate`

5. `pip install -r requirements.txt`

6. `git init`

## Build

`jupyter-book build <book-name>/`

## Development

Test build locally before deploying. Update requirements.txt to include any new packages required to build package.

## Deployment

Push changes to GitHub and GitHub Actions should do the rest.

I had to change the path for 'Upload the book's HTML as an artifact' in deploy.yml from `_build/html` to `{book-name}/_build.html`