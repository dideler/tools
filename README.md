This repo is a personal collection of projects that I build and use, but do not
necessarily contribute to.

I'm using Git + GitHub as a package manager more or less. Either because some of
these projects are not available pre-packaged via a package manager or the
available versions are outdated.

Commits like `Update <project> submodule` are personal reminders for when
I last updated *and* built the project. I try to mention the version I
last built in the commit message body.

---

- Clone this repository with `git clone --recursive` to pull in the submodule data
- Adding a shallow submodules: `git submodule add --depth=1 <path>`
  - Repos need to be unshallowed if pushing to Heroku: `git fetch --unshallow`
- Updating submodules: `git submodule foreach git pull --rebase`
- Removing a submodule: `git rm -f <submodule> && rm -rf .git/modules/<submodule>`
