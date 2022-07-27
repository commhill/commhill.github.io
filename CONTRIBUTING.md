# Contribution Guidelines for www.commhill.org

If you're not a web developer, or simply don't have time to fix an issue, please
[open a new issue](https://github.com/commhill/commhill.github.io/issues/new). In the
new issue, please include a description of what you think should be changed. After
the issue has been created, a volunteer will review it and act accordingly.

## Developer Quickstart

1. Fork the `commhill/commhill.github.io` repo as documented on [GitHub](https://docs.github.com/en/github/getting-started-with-github/fork-a-repo).
2. Clone the repo to your machine using the follwing command:
   - `$ git clone <forked-repo> --recurse-submodules`
   - If you already cloned, but forgot submodules, run `$ git submodule update --init --recursive`.
3. Install [Hugo](https://gohugo.io/getting-started/installing/) for your specific operating system.
4. Run locally:
   - `$ hugo server -D`

## Deployment

Deployment to https://www.commhill.org is automated. Everything committed to the
main branch will be deployed by Github Actions to Github Pages (the gh-pages
branch in this repo). Github Pages then sits behind Cloudflare.

Cloudflare is used for caching (especially for PDFs), various page redirects
(e.g. https://commhill.org/chat), and DNS (registration and hosting).

PDFs (https://static-www.commhill.org) are currently hosted on an Azure storage
container maintained by Jon. For discussion on this, please [see this issue](https://github.com/commhill/commhill.github.io/issues/1).
