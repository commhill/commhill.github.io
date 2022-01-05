# Contribution Guidelines for www.commhill.org

I'm really glad you're reading this, because we need volunteer developers and
general feedback to help this project come to fruition.

If you're not a web developer, or simply don't have time to fix an issue, please
[open a new issue](https://github.com/commhill/commhill-org/issues/new). In the
new issue, please include a description of what you think should be changed. After
the issue has been created, a volunteer will review it and act accordingly.

## Developer Quickstart

1. Fork the `commhill-org` repo as documented on [GitHub](https://docs.github.com/en/github/getting-started-with-github/fork-a-repo).
2. Clone the repo to your machine using the follwing command:
   - `$ git clone <forked-repo> --recurse-submodules`
   - If you already cloned, but forgot submodules, run `$ git submodule update --init --recursive`.
3. Install [Hugo](https://gohugo.io/getting-started/installing/) for your specific operating system.
4. Run locally:
   - `$ hugo server -D`

## Deployment

Deployment to https://www.commhill.org is automated. Everything committed to the master branch will be deployed by Github Actions to an Azure storage container which is then served out via Cloudflare's CDN.
