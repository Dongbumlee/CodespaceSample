[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://github.com/codespaces/new?hide_repo_select=true&ref=main&repo=920326184)

# How to make the Github Codespace Button  

## 1. Get GitHub CLI [Github CLI](https://github.com/cli/cli)  

## 2. Get Repo ID  

```gh
gh api  gh api repos/Dongbumlee/CodespaceSample --jq '.id'
```

## 3. Create GitHub Codespacee button with ID
the ID of this repo was 920326184
```
[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://github.com/codespaces/new?hide_repo_select=true&ref=main&repo=920326184)
```
