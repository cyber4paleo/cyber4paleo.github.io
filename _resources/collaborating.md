---
title: Project Management (& GitHub) for C4P Participants
layout: page
concept: Best practices for collaborating through GitHub during the development workshop.
---

By: Simon Goring

*GitHub is a collaborative environment for sharing projects among participants.  It is designed for programmers and is based on git, a program to manage version control in program development.*

*While GitHub is often used for active development of computer programs, it can be used for a range of other uses, including data management, text development/paper writing, or, really, whatever you want.*

* TOC
{:toc}

## How to Get An Account

If you already have an account then you’re set here.  Otherwise, setting up a GitHub account is fairly straightforward.  Go to [http://github.com]() and set up an account.  In general it’s best to have a shorter account name.  Any project you set up in GitHub will have a URL that includes your account name, so the shorter (and more identifiable) the better.  I’d rather go to:

[https://github.com/abcd/123]() [not a real repository]

than

[https://github.com/somereallylongusernamethatsannoyingtotype/123]() [also not real]

Once you’ve got your username, then you need to join our Development Organization.

### Best Practices

While setting up a basic account is pretty easy, there are a few things you can do to really improve your account and to get more out of GitHub as a platform.  All of the following can be accessed from the “Edit Profile” button visible from your profile page.

1. **Edit your profile**: Adding a picture or avatar to your profile is helpful to other people.  When you start contributing to a project the avatar becomes associated with each change you make or issue you raise.  GitHub provides a default avatar, but using something that’s personalized will help other people and give you higher visability.
Change your email settings: You may want to add an extra email address, make your email address private or change the things GitHub sends you.
2. **Add notifications**: When editing your profile click the “Notifications” link in the sidebar.  This enables you to receive (or not receive)  emails when things happen in repositories that you have contributed to. Adding notifications keeps you from getting “out of the loop” on a project when you’re working on something else.
Enable the Two Factor Authentication: Through the “Security” link, this helps secure your account in the same way you might for gmail or other accounts, by sending a unique PIN to a mobile device.  This helps ensure your account is more difficult to hack.  Especially if you’re using GitHub as a data/project backup you should enable this.

## How to Join a Team

At some point you will be joining one or more teams during this Development meeting.  We have created a GitHub Organization for the development meeting: 

[https://github.com/cyber4paleo]()

It’s possible for you to develop directly from your own account using a repository, but building as part of the organization lets you share credit, and, in the case that you are developing something using sensitive data, we have the ability to create Private repositories, although our strong preference is to use public repositories within the organization.

Once you’ve established your account send one of the Organization Administrators an email (currently: goring@wisc.edu) and we’ll add you to the organization.  Once you are a member of the organization you will be able to see and create new repositories and make changes to them.  The current settings do not allow you to add new members.

## Creating a GitHub Workflow

The most important point here is to be conscious of the choices you make.  Not making a choice, and putting things off for later is a choice in itself and can affect your team and its future success.

### How to Create a Repository

Once you’ve become a member of an organization & met with your team, take the time to set up a repository.  Setting up a repository is fairly simple.  Navigate to the Organization’s page (here: https://github.com/cyber4paleo) and click “New Repository”.  From here you will be asked to provide a repository name, choose whether the repository is to be public or private, decide whether you want a README and add a license and/or gitignore.

### Best Practices

1. The repository name should be simple but descriptive.  The Description should add to this (and should be filled out).
2. The repository should be Public unless there is a specific reason it needs to be Private.
3. You should generate a README file by default.
4. You should add a .gitignore for the programming language you expect to use most in the project.
5. You should generate a license.  MIT is the most permissive and is my (SJG’s) default.

<div class="boxed">
Our Project Repository is:<br><br>
</div>
<br>
<div class="boxed">
Our description is:<br><br>
</div>
<br>
<div class="boxed">
Is your repository public or private?  Why?<br><br>
</div>
<br>
<div class="boxed">
Which `.gitignore` did you choose (if any)?<br><br>
</div>
<br>
<div class="boxed">
Which license did you choose?  Why?<br><br>
</div>

## Get the Repository Onto Your Computer
Once you’ve created the repository you’ll want to get it onto your computer.  To do this you can use the GitHub Desktop application [here] or use git from the command line [here] or a number of other applications.  You will be “cloning” the repository using whichever tool you choose.  GitHub provides an explanation of how to clone a repository from ither the command line or GitHub Desktop here [link].

## Write a Good README File

A good README file is important. There is even a school of thought called “README Driven Development”.  Often times README files are nothing but the repository name, but the README is the first introduction most people will have to your repository, and so it’s important to use it to showcase the project.  In README Driven Development the philosophy rests on the fact that READMEs are limited to a single “page”, and so development stays focused on key design principles and tasks.

A good README provides a road map to the project, introduces & credits team members, provides examples of the project in action (for common uses), and provides links to outside resources.  If you develop a clean & clear README file you can use it yourself as a roadmap to project development.

The README on GitHub is written using Markdown.  There is good documentation on Markdown from GitHub [here and in more detail here], but what you really need to know is that it’s basically a plain text file that you can edit with a basic text editor.  Some suggestions include Sublime Text, Notepad, vim, emacs or Notepad++.

### Best Practices

I like to think that the neotoma package for R has a pretty good README [link].  It could be improved, but it hits some of the key points:

1. Think about what you want to do first. Then write. It’s okay to have a placeholder with something short, but a good README will reflect some thought by the team.
2. Credit your team members
3. Provide installation instructions (may be less important at first)
4. Link to help/issues/bug reporting
5. Provide contribution guidelines (or link to your Code of Conduct [link])

<div class="boxed">
Which team member will be responsible for creating the README:
<br><br>

</div>
<br>
<div class="boxed">
What are the main headings in your README?<br><br>
</div>
<br>

## Organize Your Files

You’ve thought about the project a bit in developing your README file, now think about what development will look like and how you want to organize your resources.  You want your repository to be clean & organized, for yourself and for people who might want to contribute to your project.  There are lots of good explainers for how to structure a repository or project directory because it’s really important for collaborative work.  Seriously.  Really.  I can’t emphasize it enough.  Promote someone to be your Project Manager and make one of their duties file management.  It will be helpful.

The biggest problem is a failure to maintain any sort of document hierarchy, and the second is to make single, monolithic directories.

### Best Practices

Best practices may vary by programming language, here are some for Python [link], R [link], and Ruby [link]
Maintain a document that helps organize the project.  We talked earlier about the README, but for more complex analytic workflows something like an RMarkdown document, or IPython notebook might be more useful.  You could also use a Markdown document.  Where does this file go?  In docs?  In the main repository?

<div class="boxed">
Briefly sketch your project directory structure:
<br><br><br><br><br><br><br><br>
</div>

## Decide How to Collaborate

Will you all be pushing to the same repository?  Will you be branching and making pull requests?  Will you be forking and making pull requests?  It’s best to make these decisions as a team.

GitHub has excellent documentation for collaborating through forks [here, and in more detail here], and this is, in general, my preferred way of collaborating.  This document will lay out some more detailed information about how to actually accomplish the tasks programmatically, but in general there are two models:

### Fork + Pull

Usually the model with bigger projects. GitHub provides a more extensive guide on forking, I will briefly discuss this collaboration model though. An individual makes a copy of the parent repository within their own user account, so they might fork the project:theonion/fartscroll.js to happyuser/fartscroll.js (I’m implying that [http://github.com]() comes before the user/repository format).  There the user could make changes, and, if they felt that the changes were worth incorporating back into the main repository, then they could make a Pull Request.  The main point here is that the user makes changes locally in their own account and then the changes are considered by the owner of the parent repository before incorporation.  This allows an extra degree of project management since the administrator can potentially reject changes, ask for revisions, or decide the order in which changes will be incorporated.

### Shared Repository

Here everyone uses the same repository.  This is often the case with small teams.  You pull the most recent changes to your machine, edit, and then push back to the repository, immediately incorporating your changes to the parent repository.  The reason this doesn’t make sense for larger projects is that you might have many users making simultaneous (and potentially conflicting) changes.  If you are managing the project with a small team, with good communication, this might be the easiest way to manage the project (it’s not that much harder to do it the other way though!).
A subset of this model is the Branch + Pull.  This is one of the methods that GitHub is actively advocating [here], and is a good model for users to practice.

<div class="boxed">
How will you collaborate?  Why?<br><br><br><br>
</div>

## GitHub Basics
GitHub provides an excellent “Hello World” tutorial [here] that is worth working through if you haven’t used GitHub or git before.  The following is just a brief overview of a git workflow:

### Terminology
When you work with a repository you will (in general)

1. Pull the version from a repository online to your computer
2. Make local changes
3. Commit the local changes
4. Push your local version back up to GitHub

#### The Pull

When you pull (using git pull from the command line), you are calling out to your GitHub repository and asking for the latest version of the repository.  This ensures you’re editing the most recent version of the documents.

#### The Commit

Once you’ve pulled you can edit, using whatever tool you want to use.  Once you’ve made some changes you’ll want to commit those changes.  This is your way of formalizing the changes you’ve made.  There is lots of advice on how to write a good commit message [link] and when to commit (early & often).  My general rule is to try to make “atomic” commits.  While you’re working, if you have solved a problem, added a feature, or worked on something in particular, and you’re done with it, then commit.

Especially if you’re working with others, failing to commit regularly gets you into conflict quickly, and prevents people from (1) rolling back your changes in the event of an unintended change (2) incorporating your changes in the event of a conflict and  (3) understanding what you’ve done in a systematic way.

#### The Pull

It is always good practice to pull before you push, especially if you’re working in a repository where multiple users are working simultaneously.  This lets you fix any conflicts on your end before you push them back up to the main branch.

#### The Push

Once your changes are commited & you’ve ensured that they don’t overlap you can push up to the repository.  If you are working on a branch or on a fork of the main repository then this is followed by a Pull Request.
