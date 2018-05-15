Making updates to the Palmer Lab Website

Thank you for helping with the website! This is a guide for how to make routine updates for new publications, news items, and lab members. Make sure have a github account so you can be added to the palmerlab-umd github organization and have permissions to edit the website. You can edit the website online with the "edit" button, or by cloning the repository to your computer and working locally then pushing changes back to github (you will need to have git installed). 

## Breaking things

**go to previous version of a file**
If you want to go back to a previous version of a file, you can use git to "revert" or "checkout" a previous version of that file, with the code identifying which commit you want to revert back to. To reset the file "filename" to commit "abcde", use the syntax: 

```
git reset abcde filename
git push
```

[reference](https://fettblog.eu/snippets/git/reverting-a-single-file/)

**validate YAML header**

Like spell check for code! 
[YAML validator](https://codebeautify.org/yaml-validator)

---

## Add Publications

---

## New News

To add a news item, create a new markdown (`.md`) file in the folder `_posts/labnews/` following the file name convention: **YYYY-MM-DD-Short_name_for_post.md**. The file should contain a YAML header which describes some configuration parameters, and then the text of the post. The header will look something like below - make sure to include the **labnews** category tag so the page gets created in the right place. 

```
---
author: anna
comments: true
date: 2018-04-04 12:00:00
layout: post
slug: Alec-Wetland-Tea
title: "Alec's Research Outreach Video"
categories:
 - labnews
---
```

A few places to find guidelines for GitHub's particular implementation of markdown formatting are [here](https://guides.github.com/features/mastering-markdown/) and [here](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet). To see how other news items included a photo or video, you can see the plain text version of those files online by navigating to a file in the `labnews` folder, and clicking the "**Raw**" button.  

To add a **photo** to a news item, upload your file to the "newsphotos" folder within the "img" folder. Then insert this line in your markdown file, editing the "MYPHOTO" and "PHOTO_CAPTION" and size parameters to your file name.
```
<img src="{{ site.url }}/img/newsphotos/MYPHOTO.png" alt="PHOTO_CAPTION" width="150px" hspace="20px">
```
---

## People updates

To edit information about lab alums, edit `team/index.html` ([link](https://github.com/palmerlab-umd/palmerlab-umd.github.io/blob/master/team/index.html)). There is a list starting around line 48 after the line `lab_alumni:`. Each line needs to begin with `- name: `. 

Enhancement: To automate link formatting, edit the layout instructions at the bottom of the page under ` {% for student in page.lab_alumni %}`

---
