---
layout: post
title: How to manage environment using conda
category: python
---

This post will guild you how to create and manage conda environment

## What is conda environment?

## List all environment

To list all environment in your computer, open Anaconda Command Prompt and type in:

`conda info --envs`

![List conda environments](https://harryteststorageblob.blob.core.windows.net/blogazureimage/Image/anaconda/anaconda_list_envs.png)


## Create new environment

To create new environment using **conda**, open Anaconda Command Prompt and type in:

`conda create --name your-env-name python=3.7 -y`

or

`conda create -n your-env-name python=3.7 -y`

With this command conda will copy all the base packages of python 3.7 versions to the new environment.

## Active new environment

We need to active the environment to run a package from that specific environment or de

## Deactive environment

If we deactive environment, conda will return to the base environment.

`conda deactivate `

## Delete environment


**Reference**: https://kapeli.com/cheat_sheets/Conda.docset/Contents/Resources/Documents/index