# Docusaurus git submodules tests

Related to:
- https://github.com/e18e/ecosystem-issues/issues/216
- https://github.com/facebook/docusaurus/issues/11208
- https://github.com/facebook/docusaurus/pull/11512

---

## Creation

Repo created with 3 submodules:

```bash
git submodule add git@github.com:facebook/docusaurus.git docusaurus
git commit -m "Add Docusaurus submodule"

git submodule add git@github.com:facebook/react-native.git react-native
git commit -m "Add React Native submodule"

git submodule add git@github.com:facebook/react-native-website.git react-native-website
git commit -m "Add React Native Website submodule"

git push
```

---

## Cloning

Clone the repo, including its submodules

```bash
git clone --recurse-submodules git@github.com:slorber/docusaurus-git-submodules-tests.git
```

If you already cloned the repo without submodules, you can run:

```bash
git submodule update --init --recursive
```

## Useful commands

List submodules:

```bash
git submodule
```

Get the repository root dir:

```bash
git rev-parse --show-toplevel
```

Get the "superproject" path from a submodule cwd:

```bash
git rev-parse --show-superproject-working-tree
```
