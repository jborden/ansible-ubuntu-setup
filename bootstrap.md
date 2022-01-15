# Boot Strap
This is a list of things that were done just to get a
minimum environment to first create the ansible file.

once the initial ansible file is created, backfill these
tasks.

# Emacs
emacs was installed
```
sudo apt install emacs
```

.emacs file was copied to ~/
the best solution for this will likely be a git sub module
so that .emacs is kept downloaded to emacs/files/emacs
```
cp emacs .emacs
```

## Fonts

emacs was dependent upon monaco font being installed
https://askubuntu.com/questions/333409/how-to-install-the-monaco-font

note that the download was used.
https://askubuntu.com/questions/333409/how-to-install-the-monaco-font/906181#906181

This should be done by Ansible

## use-package issues

There were issues with use-package not being installed
```
(package-install 'use-package)
```
was used. The .emacs file needs to be more robust for fresh installations

## cider and other clojure packages not working
there is an issue with 'map-2' package not being available.
could be due to poor internet connectivity, but this should be explored.

# git

git needs to have an email set before it can be used.


```
git config --global user.name "James Borden"
git config --global user.email "jmborden@gmail.com"
```
