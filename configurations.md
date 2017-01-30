---
title: Configurations
layout: main
---

When I install a new operating system, I commit to spending a decent amount of time
getting **everything** configured ahead of time that I can.  As we continue forward with
the course I will add more descriptions as we learn more tools.  It is **very
important** that you understand two things:

1. These configurations are what work for me.  What I prefer may be uncomfortable for
   you, or may not be as efficient for you as it is for me.
2. I in no way learned / memorized all of these at once.  Whether it is aliases I use in
   my terminal, or shortcuts I use for text editors, do not try and just "know them all".
   Instead, while you get used to things, choose a subset to train yourself with and
   when you get comfortable with that subset start bringing in more.

I cannot emphasize enough the value in configuring things yourself.  From colors, to the
shell you use, to what hotkeys you prefer in your Operating System, they only take
meaning if they help you _and_ you remember them.  This list comes from a few years of
me cultivating / changing aspects of my development environment.

Basically, you should plan on changing the below to work for you, not just use it
because it is here.

# First things First
----------------------------------------------------------------------------------------

Make sure you have the base operating system as up to date as possible, and install some
core development tools.  When you perform a fresh installation, there usually have been
quite a few updates between what was packaged into the media you just installed (e.g.
the `.iso` you acquired), and what is available online right now.

All in all, there are three **fundamental** elements of development I will be teaching
you:

1. Being comfortable functioning in your terminal.
2. Using version control (we will use `git` in this course).
3. Understanding how to use both a terminal based text editor (we will be learning `vim`
   in this course), and a GUI-based editor.
    - I prefer [Sublime Text](https://www.sublimetext.com/), but there are many options.
      The point is that you will probably prefer to use your GUI-based editor / IDE, but
      will also need to be able to edit files from your terminal.

{% include configurations/tri_template.html name='first_things_first' %}


# Workspaces and Overall Appearance
----------------------------------------------------------------------------------------

In my experience, the single most useful thing to configure for a development
environment is "Workspaces".  I am not alone in this -- as of 2017 it's pretty much the
defacto standard for an operating system to include workspaces.  Virtually every desktop
manager available for Linux has them, and Windows and Mac also include them too!

<div class="panel-group" id="what_are_workspaces">
  <div class="panel panel-default">
    <div class="panel-heading">
      <h4 class="panel-title"><a data-toggle="collapse" data-parent="#what_are_workspaces" href="#what_are_workspaces_inner">
        Click for How I Use Workspaces
      </a></h4>
    </div>
    <div id="what_are_workspaces_inner" class="panel-collapse collapse">
      <div class="panel-body">
        {% assign what_are_workspaces = 'configurations/workspaces_and_overall_appearance/what_are_workspaces.md' %}
        {% capture workspaces_include %}{% include {{ what_are_workspaces }} %}{% endcapture %}
        {{ workspaces_include | markdownify }}
      </div>
    </div>
  </div>
</div>

Since the tools that we will install to get workspaces give us other options to
customize our appearance, we'll go ahead and get those setup at the same time.

{% include configurations/tri_template.html name='workspaces_and_overall_appearance' %}
