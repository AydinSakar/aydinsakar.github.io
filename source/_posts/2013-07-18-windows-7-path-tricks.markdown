---
layout: post
title: "Windows 7 Path Tricks"
date: 2013-07-18 12:33
comments: true
categories: 
- Windows 7
- Path
---

There are a number of things to remember when you deal with the `Path` environment variable in Windows.

1. The items in the `Path` string are seperated by semicolon: `;`, there should be no space around the semicolon. "C:\SomePath ; C:\AnotherPath" is **NOT** OK.

2. It is better to use `\` instead of any `/` in the string.

3. No final backslash as in: `C:\SomeDirectory\`.

4. Whenever you make a change to `Path` variable, be sure to close and reopen any Cmd or Shell window.

5. You can add a new environment variable as "myexedir" and add that variable as ;%myexedir% to the Path string.

6. Open cmd.exe with administrator privileges and type:

    setx path "%path%;C:\Python27" /m

`/m` makes the changes at the `system environment`, if you omit it then the changes are made in the `local environment`.

7. Nonexisting paths in `Path` can cause problems.

8. [Path Manager](http://pathmanager.sourceforge.net/) is a little utlity that helps with the `Path` problems.

9. You can prepare a bat file:

    @echo off
    PATH C:\Python27;%path%
    title Octopress - %Username%@%Computername%
    cd C:\Projects\WebProjects\octopress
    cmd

Which will add the directory you want to be added to the Path. This will be valid for the command session only, and as a bonus can land you right into the directory that you want to work. This solution is the one that I feel more comfortable with.

For a discussion about these recommendations on [Stackoverflow](http://stackoverflow.com) see: <http://stackoverflow.com/questions/6318156/adding-python-path-on-windows-7>
