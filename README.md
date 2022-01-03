# A weakly structured stem for human origins in Africa

This repository contains the manuscript and supplementary material for "A
weakly structured stem for human origins in Africa." To build the document,
simply type `make` in this directory. If you have only updated the supplement,
you may need to type `make -B` instead to force a rebuild.

GitHub is set up to automatically build the manuscript from the most recent
commit, and PDFs of the paper and supplement can be found
[here](https://apragsdale.github.io/african-structure-paper/PDFs.html).

## Getting started

You may need to install `pdflatex` to compile the document.

On linux:

```sh
sudo apt-get install texlive-latex-base texlive-fonts-recommended texlive-fonts-extra texlive-latex-extra
```

On mac (untested):

```sh
brew install basictex
```

## Contributing

You can make small edits in the browser by navigating to the file and clicking
the "edit" button (which looks like a pencil in the top-right corner of the
window). Any edits you make can then be committed directly to the repository
by completing the "Commit changes" section at the bottom of the page. Just include
a short phrase saying what you edited and click the green "Commit changes" button.

To make larger edits and to compile the document, you should first clone the
repository to your own computer, make changes there, commit the changes locally,
and then push those changes back to the repository.

*Note: It's best to make small commits and push often to ensure conflicts don't
arise. Also, it's helpful to coordinate to make sure only one person is tackling
a given section at a time to avoid merge conflicts.*

### To clone the repo
```sh
cd Documents  # or wherever you want this project to live locally
git clone git@github.com:apragsdale/african-structure-paper.git
cd african-structure-paper
make
```

### To push your recent edits to the repo
After editing some section, do the following
```sh
git add [files-you-edited]
git commit -m "very short message describing the edits"
git push origin main
```

### Making sure your copy is up to date
If you've already cloned the repository, you want to make sure you are editing
the most up-to-date version of the document. Before doing any editing, pull
changes from the repository:
```sh
git pull origin main
```

### What to do in case of conflicts
The best way to avoid conflicts is to always make sure you are working with the
most up to date version of the document, by pulling from the repo (see section
above). But it can sometimes happen that someone else has pushed changes to the
repo in the time between pulling and pushing changes yourself. In that case,
pushing the repo might generate a message that says something like
```sh
 ! [rejected]       main -> main (fetch first)
 error: failed to push some refs to `github.com:apragsdale/african-structure-paper.git`
```
as well as some extra lines that have a hint.

To be able to push the changes in this case, you need to pull and merge the more
recent changes from the repo:
```sh
git pull origin main
```
With any luck, everything merges properly, and you can try pushing againg
```sh
git push origin main
```
