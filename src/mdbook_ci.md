> Captain's log, Stardate **2122.275.5**

# Notes on CI/CD for mdbook

## Setting up gh-pages and build-test github action
Easy deployment of mdbook to gh-pages.

- Setup gh-pages for the repo
    - Create a branch `gh-pages`
    - settings (repo) -> Pages -> set source as branch `gh-pages` and location `root`
- [Follow this reference](https://github.com/peaceiris/actions-mdbook#getting-started).
- Don't need to modify this line, `github_token: ${{ secrets.GITHUB_TOKEN }}`. A GitHub Actions runner automatically creates a GITHUB_TOKEN secret to authenticate in our workflow
- Make changes regarding the branch name the yml file, if required.

Finally a reference of the [logbooks's CI/CD workflow](https://github.com/madclaws/madclaws.github.io/blob/master/.github/workflows/logbook.yml)