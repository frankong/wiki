How to use Git
===============


Clone::
  
  git clone https://github.com/mrirecon/bart.git
  git clone --recursive git://github.com/foo/bar.git

Fetch upstream::
  
  git remote add upstream https://github.com/mrirecon/bart.git


Submodule::
  
  git submodule add https://github.com/mrirecon/bart.git

  git submodule update --init --recursive

Subtree

add::
  
  git remote add bart https://github.com/frankong/bart.git
  git subtree add --prefix=c/bart https://github.com/frankong/bart.git master

pull::
  
  git subtree pull --prefix c/bart/ --squash bart master
