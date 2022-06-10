# Documentation

## Checkout and build

```
git clone git@github.com:CMSRKR3/tdr.git notes
cd notes
git submodule init
git submodule update
cd AN-21-XXX
. build.sh
```

## Adding the utils submodule

Just for reference, to be done once only on the creation of this repo.

```
# https://git-scm.com/book/en/v2/Git-Tools-Submodules
git clone git@github.com:CMSRKR3/tdr.git notes
cd notes
git submodule add ssh://git@gitlab.cern.ch:7999/tdr/utils.git
git diff --cached --submodule
git ci -am "Add utils submodule"
git push origin main
```
