# Quiz on Git

## What you should do:

1. Create a branch with your name and commit your changes to it.
2. **To check the correct answers**: edit the README document and replace the ``[ ]`` with ``[x]`` to mark the correct answers.

Question 1
----------
After you initialize a new Git repository and create a file named ``my_file.txt``, which of the following commands will not work if issued?

- [ ] git status
- [ ] git add .
- [X] git commit -m "my_file.txt is added"
- [ ] git add my_file.txt

Question 2
----------
Say you have three changed files (``README.md``, ``my_code.py`` and ``my_page.html``) that are not staged yet. You want **only** to commit the changes of the file ``my_page.html``, you'll perform the following:

- [] execute the following commands:

    1. git add .
    2. git commit -m "added the file my_page.html"

- [ ] execute the following commands:

    1. git add my_page.html
    2. git commit -m "my commit message"

- [X] execute the following commands:

    1. git add my_page.html
    2. git commit -m "added the file my_page.html"

Question 3
----------

Which command should you use to initialize a new Git repository?

- [ ] git bash
- [ ] git install
- [X] git init
- [ ] git start

Question 4
----------

Which file can you configure to ensure that certain file types are never committed to the local Git repository?

- [ ] ignore.git
- [ ] .gitignore
- [ ] gitignore.txt
- [X] git.ignore

Question 5
----------

When you run the command ``git branch debugging``, the following will happen:

- [ ] The ``HEAD`` will point to the newly created branch named ``debugging``
- [ ] Create a new branch named ``debugging`` and you'll see the message: ``Switched to branch 'debugging'``
- [X] Create a new branch named ``debugging`` and ``HEAD`` will stay pointing at ``master``   
- [ ] None of the above


Question 6
----------
Consider you start with an **empty** directory and you initialize a git repository. After a couple of commits and branchings you end up with the following history:

![](graphics/quiz_p5.png)

The commits C<sub>1</sub>, C<sub>2</sub>, ... are numbered in sequence, which means that the commit C<sub>1</sub> came before the commit C<sub>2</sub> and the commit C<sub>3</sub> before C<sub>4</sub>. The commands that were performed to get the to this **exact history** are the following:

- [X] After ``git init`` and the first commit C<sub>1</sub>:

      1. git checkout -b debugging
      2. modify  and commit
      3. git checkout -b testing
      4. modify  and commit
      5. git checkout debugging
      6. modify  and commit
      7. git checkout testing
      8. modify  and commit
      9. git checkout master
      10. modify  and commit

- [ ] After ``git init`` and the first commit C<sub>1</sub>:

      1. git checkout -b debugging
      2. git checkout -b testing
      3. modify  and commit
      4. modify  and commit
      5. git checkout debugging
      6. modify  and commit
      7. git checkout testing
      8. modify  and commit
      9. git checkout master
      10. modify  and commit

- [ ] After ``git init`` and the first commit C<sub>1</sub>:

      1. git checkout -b debugging
      2. git checkout -b testing
      3. modify  and commit
      4. modify  and commit
      5. modify  and commit
      6. git checkout debugging
      7. modify  and commit
      8. git checkout master
      9. modify  and commit

- [ ] After ``git init`` and the first commit C<sub>1</sub>:

      1. git checkout -b debugging
      2. modify  and commit
      3. modify  and commit
      4. git checkout -b testing
      5. modify  and commit
      6. git checkout debugging
      7. modify  and commit
      8. git checkout master
      9. modify  and commit

Question 7
----------
You have three files in your working directory: `.gitignore`, `A.txt`, `B.txt` and `code.py`. The file `.gitignore` contains the following: `*.txt`. We run the following commands:

1. git add *
2. git commit -m "added all the files"
3. git push --set-upstream origin master

Do you think that all the files will be pushed to the remote? Explain why.
No, only the "code.py" will be pushed to the remote since the rest are (.txt) 


Question 8
----------
Given the following scenario:

               HEAD (refers to branch 'master')
                |
                v
a---b---c---d  branch 'master' (refers to commit 'd')
    ^
    |
  tag 'v2.0' (refers to commit 'b')

Where will the HEAD point if we run the following command:
``git checkout v2.0``

Answer:
the comment git checkout "branch name" swithces to the targeted branch(the name of the branch we insert)
then the head point will be at point b.

Question 9:
----------
Consider the following scenario:

![](graphics/quiz-p9.png)

Explain what will happen when we run the following commands:

1. git checkout experiment 
the head will point to the experiment
2. git rebase master
master will point to the experiment 
3. git checkout master
master points to experiment then the head will remain pointting  to experiment 
4. git merge experiment


You need to specify where ``HEAD``, ``master`` and ``experiment`` will be after these commands, and you need to sketch theupdated history. You may add a graph as an answer in a folder named as follows: ``firstName_LastName_graphics``.

Question 10:
-----------
We know that instead for adding then commiting, we can use the command ``git commit -m "my message" -a``. Here the ``-a`` flag adds all the modified files then do the commit.
Suppose the following scenario: in the working directory, everything in up-to-date with your git repository. Now you create a new file named ``code.py``. Then to put it under version control, you run the following:

``git commit -m "added code.py" -a``

Is this correct? Explain why.

It's correct
