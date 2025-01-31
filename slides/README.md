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
See [hash for template](https://github.com/mxochicale/open-healthcare-slides/commit/185b5a53fdfe32f3ff98de0734f54cd2c471183c)

* Select deploy from branch and select gh-pages


## Edit and preview slides

### Dependencies
* quarto installation (Reference https://quarto.org/docs/download/tarball.html).
```
mkdir -p ~/opt && cd ~/opt
wget https://github.com/quarto-dev/quarto-cli/releases/download/v1.5.57/quarto-1.5.57-linux-amd64.tar.gz
tar -C ~/opt -xvzf quarto-1.5.57-linux-amd64.tar.gz
mkdir -p ~/.local/bin
ln -s ~/opt/quarto-1.5.57/bin/quarto ~/.local/bin/quarto
( echo "# local/bin/quarto from ln -s /opt/quarto*"; echo 'export PATH=$PATH:~/.local/bin' ; echo "" ) >> ~/.bashrc
source ~/.bashrc
quarto check
```

### Quarto extensions
```
quarto list extensions
quarto add parmsam/quarto-subtitles
quarto remove parmsam/subtitles
#https://github.com/parmsam/quarto-subtitles
```

### Edit and preview slices
* Open [index.qmd](index.qmd) to edit slides. 
* Then you can preview them:
```
cd slides
quarto preview index.qmd
```

## References
* https://quarto.org/docs/presentations/revealjs/
* https://quarto.org/docs/presentations/revealjs/advanced.html

