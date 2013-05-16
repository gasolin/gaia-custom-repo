gaia-custom
===========

Experiment of using repo to manage gaia with customize distribution

Create a dir

    $ mkdir mozgaia
    $ cd mozgaia

init repo

    $ repo init -u https://github.com/gasolin/gaia-custom-repo.git

sync repo

    $ repo sync
    

## For Gaia Developers

Here's howto make your own dev repo settings for experiment:

1. Fork https://github.com/gasolin/gaia-custom-repo.git
2. edit default.xml , replace remote to your repository (ex: mine gaia is at 

     <remote name="b2g" fetch="https://github.com/gasolin/"/>

3. comment out `project remote="yurenju"` if you don't need customization

4. then sync the project

    $ repo sync

That command will download all required .git for you.

## Reference

* Git and repo cheatsheet http://source.android.com/source/developing.html#git-and-repo-cheatsheet
