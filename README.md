# Docusaurus git submodules tests

Related to:
- https://github.com/e18e/ecosystem-issues/issues/216
- https://github.com/facebook/docusaurus/issues/11208
- https://github.com/facebook/docusaurus/pull/11512

Repo initialized with:

```bash
git submodule add git@github.com:facebook/docusaurus.git docusaurus
git commit -m "Add Docusaurus submodule"

git submodule add git@github.com:facebook/react-native.git react-native
git commit -m "Add React Native submodule"

git submodule add git@github.com:facebook/react-native-website.git react-native-website
git commit -m "Add React Native Website submodule"

git push
```
