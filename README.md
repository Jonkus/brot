
BROT
====

## Installation ##

 1. Configure your paths in config.def
 2. Run the _./build_ script

## Overview ##

#### What is brot? ####

Our goal is to create a minimal yet functional blogging engine. The usage of
standard unix tools like awk or sh allows us to archive tasks others need 
bloat-ware for.

#### How does it work? ####

The heart of brot is a git repository containing your blog-articles. You can 
thus checkout this repostitory and commit new blog entries or change them.
By pushing your changes a git-hook is executed which converts your 
markdown-files into html and adds an index entry.

With the help of mehl you can also send an e-mail with your article as
plain/text to a functional e-mailbox. Mehl then commits and pushes it to the 
blog-repository, so the new entry appears. (tbd)

## Usage ##

 1. _git clone [blog-repository-location]_
 2. make your changes and additions (mainly in config.def)
 3. commit und push to your repo

     - public-branch deploys in the _DEPLOYMENT\_DIR_
     - private-branch deploys in the _PRIVATE\_DEPLOYMENT\_DIR_

 4. watch your generated html-files in your deployment-path

## ToDo's ##

 - including mehl
 - full utf-8 support

