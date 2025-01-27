=============================
 Simple Vim templates plugin
=============================
:Author: Adrian Perez <aperez@igalia.com>

This is a simple plugin for Vim that will allow you to have a set of
templates for certain file types. It is useful to add boilerplate code
like guards in C/C++ headers, or license disclaimers.

About this fork
===============
This vim-templates fork is to add some taskwiki-specific templates and configurations, so that taskwarrior users 
can more easily start using taskwiki (+vimwiki, +two) to make "instant" project.wiki files. 

Taskwiki/ Vimwiki/ Taskwarrior Specific Notes:
============================================

To "instantly" start a project taskwiki/vimwiki file, simply enter;

    vi ~/path/name.project.wiki
    
and, for proj:name, the file will open pre-populated with metadata, project headings and pending/scheduled/completed tasks in ViewPorts. The templates are easy to customize.

Wiki templates;
-------------------
* =template=.area.wiki

* =template=.index.wiki

* =template=.project.wiki

* =template=.tag.wiki

Wiki-related user-defined variables and configs
----------------------------------
(in ../extra/taskwiki-template.vim)

%NULL$   (required to inhibit taskwiki while editing template)

screenshot:



Installation
============

The easiest way to install the plugin is to install it as a bundle.
For example, using Pathogen__:

1. Get and install `pathogen.vim <https://github.com/tpope/vim-pathogen>`_. You can skip this step
   if you already have it installed.

2. ``cd ~/.vim/bundle``

3. ``git clone git://github.com/aperezdc/vim-template.git``

__ https://github.com/tpope/vim-pathogen

Bundle installs are known to work fine also when using Vundle__. Other
bundle managers are expected to work as well.

__ https://github.com/gmarik/vundle


.. important:: If you use Fish__ as your shell, you *will* need to add
   ``set shell=/bin/sh`` to your ``~/.vimrc`` — the plugin relies on the
   setting pointing to a Bourne-compatible__ shell.

__ http://fishshell.com/
__ https://en.wikipedia.org/wiki/Bourne_shell


Documentation
=============

The documentation can be browsed directly in Vim::

    :help template.txt

Alternatively, you can also `read it in your browser`__.

__ https://github.com/aperezdc/vim-template/blob/master/doc/template.txt


Updating
========

Manually
--------

In order to update the plugin, go to its bundle directory and use
Git to update it:

1. ``cd ~/.vim/bundle/vim-template``

2. ``git pull``


With Vundle
-----------

Use the ``:BundleUpdate`` command provided by Vundle, for example invoking
Vim like this::

  % vim +BundleUpdate

