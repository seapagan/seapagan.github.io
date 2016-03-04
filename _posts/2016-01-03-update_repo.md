---
title: Update_Repo
tagline: "A Simple Gem to keep multiple cloned Git Repositories up to date"
#homepage: ""
repo: "seapagan/update_repo"
---

[![Gem Version](https://badge.fury.io/rb/update_repo.svg)](https://badge.fury.io/rb/update_repo) [![Build Status](https://travis-ci.org/seapagan/update_repo.svg?branch=master)](https://travis-ci.org/seapagan/update_repo)

This is the conversion to a Gem of one of my standalone Ruby scripts. Still very much work in progress, but functions as required.

#### Pre-requirements

It goes without saying that at the very least a working copy of both [`Git`][git] and [`Ruby`][ruby] need to be installed on your machine. Also, the script has only been tested under Linux, not windows.

[git]: http://git-scm.com
[ruby]: http://www.ruby-lang.org

#### Quick start
Create a [YAML](http://yaml.org/)-formatted configuration file `.updatereporc` **in your home directory** that contains at least a 'location' tag pointing to the directory containing the git repositories you wish to have updated :

{% highlight yaml %}
---
location:
- /media/myuser/git-repos
- /data/RepoDir
{% endhighlight %}

This is the most basic example of a configuration file and there are other options that can be added to fine-tune the operation - see the description of configuration options on the script homepage.

This file should be located in the users home directory (`~/.updatereporc`).

Run the script :
```
$ update_repo
```
