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

---

## People updates

To edit information about lab alums, edit `team/index.html` ([link](https://github.com/palmerlab-umd/palmerlab-umd.github.io/blob/master/team/index.html)). There is a list starting around line 48 after the line `lab_alumni:`. Each line needs to begin with `- name: `. 

Enhancement: To automate link formatting, edit the layout instructions at the bottom of the page under ` {% for student in page.lab_alumni %}`

---
