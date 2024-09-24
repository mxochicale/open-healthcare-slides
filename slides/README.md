# Setting up slides in quarto and github
The following are few steps to setup your quarto slides in github pages.

*  Create templates, ci workflows, code of conduct, contributions and slides
```
$ tree 
.
.
├── CODE_OF_CONDUCT.md
├── CONTRIBUTING.md
├── docs
│   ├── poster.pdf
│   ├── poster.png
│   └── README.md
├── LICENSE
├── README.md
└── slides
    ├── _extensions
    │   └── quarto-ext
    │       └── fontawesome
    │           ├── assets
    │           │   ├── css
    │           │   │   └── all.css
    │           │   └── webfonts
    │           │       ├── fa-brands-400.ttf
    │           │       ├── fa-brands-400.woff2
    │           │       ├── fa-regular-400.ttf
    │           │       ├── fa-regular-400.woff2
    │           │       ├── fa-solid-900.ttf
    │           │       ├── fa-solid-900.woff2
    │           │       ├── fa-v4compatibility.ttf
    │           │       └── fa-v4compatibility.woff2
    │           ├── _extension.yml
    │           └── fontawesome.lua
    ├── favicon.svg
    ├── figures
    │   └── 00_template-vector-images
    │       ├── drawing-v00.svg
    │       └── README.md
    ├── index.qmd
    ├── _quarto.yml
    └── README.md

10 directories, 24 files
```


* first commit
```
git add .
git commit -m ':fire: 1st commit: adds scalfolding for slides #0'
git branch -M main
git push -u origin main
```

* Create gh-pages branch
```
git checkout --orphan gh-pages 
#An orphan branch is not connected to the other branches and commits, and its working tree has no files at all. 
#See [here](https://git-scm.com/docs/git-checkout) for more info.
git reset --hard
git commit --allow-empty -m "Initializing gh-pages branch"
git push origin gh-pages
git checkout main
#https://jiafulow.github.io/blog/2020/07/09/create-gh-pages-branch-in-existing-repo/
```

* Select deploy from branch and select gh-pages

## Preview slides

### Dependencies
```
sudo apt install npm
npm install reveal.js
```

### Preview slices
```
npm start
npm stars -- --port=8001
```
