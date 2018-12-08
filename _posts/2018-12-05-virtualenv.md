---
layout: post
title:  "Python virtualenv"
date:   2018-12-05 9:00:28 -0500
categories: python devops
---


Python virtualenv is a commonly used practice to separate your python projects from one another. It can be very helpful when you have multiple projects on a local machine that have competing requirements on using different versions of a same library.

### verify if virtualenv is installed

There is a chance that virtualenv is already installed on your system. Run `virtualenv --version` in your terminal. If it is not installed, run `pip install virtualenv` (DO NOT sudo) to install virtualenv.

### prep a project folder using virtualenv

First, create a directory for a new isolated environment, say `mkdir ~/proj1_env`, and then `virtualenv ~/proj1_env` will prep the folder ready.

### use virtualenv

To begin working with your project, you go into your project directory and activate the virtual environment.

```
cd ~/proj1_env/bin
source activate
```

To exit your virtualenv just type `deactivate`

### What does virtualenv do behind the scene
Any packages you install now using pip get installed into proj1_env/lib/python2.7/site-packages, given python 2.7 is what you are using.

Packages installed here will not affect the global Python installation. Virtualenv does not create every file needed to get a whole new python environment. Instead, it uses links to global environment files instead in order to save disk space end speed up your virtualenv. 

Therefore, there must already have an active python environment installed on your system.

*References*
<https://chriswarrick.com/guides/> has some good articles regarding setting up python dev environment.
