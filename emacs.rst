How to upgrade to the latest Emacs
====================================


Mac
----

Reference: https://github.com/railwaycat/homebrew-emacsmacport

If you'd like to install with Homebrew, please::

  $ brew tap railwaycat/emacsmacport

and then::

  $ brew install emacs-mac


Ubuntu
------

Reference: http://askubuntu.com/questions/598985/how-to-upgrade-to-the-latest-emacs

You can install the nightly packages from the ubuntu-elisp ppa::

  sudo add-apt-repository ppa:ubuntu-elisp/ppa
  sudo apt-get update
  sudo apt-get install emacs-snapshot
