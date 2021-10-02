> Captain's log, Stardate **2122.275.5**

# Notes on CI/CD for mdbook

## Setting up gh-pages and build-test github action
Easy deployment of mdbook to gh-pages.

- Setup gh-pages for the repo
    - Create a branch `gh-pages`
    - settings (repo) -> Pages -> set source as branch `gh-pages` and location `root`
- [Follow this reference](https://github.com/peaceiris/actions-mdbook#getting-started).
- Remeber to create a `TOKEN` for the repo, under Settings(repo) -> Secrets
    - Add any unqiue id and give a labels, ex `REPO_TOKEN`
- Make changes regarding the branch name, token name in the yml file, if required.

Finally a reference of the [logbooks's CI/CD workflow](https://github.com/madclaws/madclaws.github.io/blob/master/.github/workflows/logbook.yml)