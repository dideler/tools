This repo is a personal collection of projects that I build and use, but do not
necessarily contribute to.

I'm using Git + GitHub as a package manager more or less. Either because some of
these projects are not available pre-packaged via a package manager or the
available versions are outdated.

---

- Only add shallow submodules: `git submodule add --depth=1 <path>`
- Repos need to be unshallowed if pushing to Heroku: `git fetch --unshallow`
- To update submodules: `git submodule foreach git pull`
  - Alternatively: `git submodule update --remote --merge --depth=1`
