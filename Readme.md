# Blog setup

## Hugo setup
install golang as local build tool: https://go.dev/doc/install
install VS Code IDE: https://code.visualstudio.com/download

go to this repo and do steps from installation link: https://gohugo.io/installation

## Theme setup

```sh
# Install:
git submodule add --depth=1 https://github.com/adityatelange/hugo-PaperMod.git themes/PaperMod
git submodule update --init --recursive # needed when you reclone your repo (submodules may not get cloned automatically)

# update
git submodule update --remote --merge
```

go to this repo and do steps from PaperMod - Installation link: https://github.com/adityatelange/hugo-PaperMod/tree/master

`install theme as shown in Method 2: git submodule add --depth=1 https://github.com/adityatelange/hugo-PaperMod.git themes/PaperMod`

`copy and paste config.yml to the root of the repo: https://github.com/adityatelange/hugo-PaperMod/wiki/Installation#sample-configyml`

Do necessary configuration of `config.yml` file

`copy and paste post template to archetypes/post.md file: https://github.com/adityatelange/hugo-PaperMod/wiki/Installation#sample-pagemd`

## Test your blog

```sh
# create new post
hugo new --kind post Hello.md

# run Hugo server and try to find your post
hugo server

# site runs at address http://localhost:1313/, just 'command + click'
```

## Blueprint pipeline

https://github.com/actions/starter-workflows/blob/main/pages/hugo.yml