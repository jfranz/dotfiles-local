jfranz dotfiles-local
===============

I use [thoughtbot/dotfiles](https://github.com/thoughtbot/dotfiles) and
jfranz/dotfiles-local together using [the `*.local` convention][dot-local].

[dot-local]: http://robots.thoughtbot.com/manage-team-and-personal-dotfiles-together-with-rcm

This is based on [Croaky dotfiles](https://github.com/croaky/dotfiles).

Requirements
------------

Set zsh as my login shell.

    chsh -s /bin/zsh

Install [rcm](https://github.com/mike-burns/rcm).

    brew tap thoughtbot/formulae
    brew install rcm

Install
-------

Clone onto my laptop:

    git clone git://github.com/jfranz/dotfiles-local.git

Install:

    env RCRC=$HOME/code/dotfiles-local/rcrc rcup

This will create symlinks for config files in my home directory.

I can safely run `rcup` multiple times to update.

What's in it?
-------------

[sublime](http://www.sublimetext.com/3) configuration:

* subl customizations TBD

[git](http://git-scm.com/) configuration:

* `l` alias for tight, colored, log output.
* `glog` alias for graphed log output.
* `gs` alias for -sb status.
* My name and email.

[zsh](http://zsh.sourceforge.net/FAQ/zshfaq01.html) configuration and aliases:

* `c` to cd into projects directory.
* `restart-postgres` alias to restart Homebrew'd Postgres.
* `install-missing-ruby` alias to upgrade Homebrew'd `ruby-build` and install
  Ruby implicitly from `.ruby_version` file in current directory.
* `nom` reset npm modules
* `nombom` reset npm and bower dependencies
