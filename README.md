
BROT
====

## Installation ##

 1. Edit _config.def_
 2. Run the _./install_ script

## Overview ##

#### What is buch? ####

Our goal is to create a minimal yet functional blogging engine. The usage of
standard unix tools like awk or sh allows us to archive tasks others need 
bloat-ware for.

#### How does it work? ####

The heart of buch is a git repository containing your blog-articles. You can 
thus checkout this repostitory and commit new blog entries or change them.
By pushing your changes a git-hook is executed which converts your 
markdown-files and generates an index.

Mehl you can also send an e-mail with your article as
plain/text to a functional e-mailbox. Mehl then commits and pushes it to the 
blog-repository, so the new entry appears. (tbd)

## Usage ##

 1. Put your markdown files into the pages/ directory of your working copy ($WORKINGCOPY) 
 2. Add, commit and push your changes to your bare repository ($BAREREPOSITORY)
  a. public-branch du in the _DEPLOYMENT\_DIR_
  b. private-branch deploys in the _PRIVATE\_DEPLOYMENT\_DIR_

 4. watch your generated html-files in your deployment-path

## TODOs ##

 - brot should be called buch. refactoring needed.
 - support for attachments in mehl
 - a bare repo can be dropped in a local environment
   installation script should support this

