gaia-custom-repo
=================

Experiment of using repo to manage gaia with customize distribution

### Install repo tool

Reference to 
* [http://source.android.com/source/downloading.html#installing-repo] (http://source.android.com/source/downloading.html#installing-repo)

### init repo

Create a directory

    $ mkdir mozgaia
    $ cd mozgaia

init the repo

    $ repo init -u https://github.com/gasolin/gaia-custom-repo.git

### sync repo

    $ repo sync
    

## For Gaia Developers

Here's howto make your own dev repo settings for experiment:

1. Fork https://github.com/gasolin/gaia-custom-repo.git
2. edit default.xml , add a remote to your repository, ex: 

     <remote name="gasolin" fetch="https://github.com/gasolin/"/>

  2.1 replace `project remote="b2g"` to `project remote="<your name>"`, ex 

      <project remote="gasolin" name="gaia" path="."/>

  2.2 comment out `project remote="yurenju"` if you don't need customization

3. then sync the project

    $ repo sync

That command will download all required .git for you.

## Reference

* Git and repo cheatsheet http://source.android.com/source/developing.html#git-and-repo-cheatsheet
