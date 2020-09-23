
## Make and clone repository 
1.	Make a new repository in your Github account called ‘test-repo’. If you already have one called this name then call it something else. Tick the initialise with README button in the options

2.	Clone the repository onto your computer using git clone. First click the green ‘code’ button in the repository on github. Copy the url inside the clone with https box 

3.	In git bash or on your linux terminal, type 
```
git clone <url>
```

## Make, stage, commit and push changes 

4.	Make some changes to the readme file by adding some text 
5.	Stage the readme file 

```
git add README.md
```

6. Commit the README.md file
```
git commit -m “ added text to README.md” file 
```

7. Push the changes to the remote repository
```
git push -u origin master
```

## Create a branch, make changes, push changes and merge branch 

8. Go to your repository in github, refresh the page and you should see your changes there

9. Click the 'commits' button on the right hand side and click into your commit message to see the changes to that file. Green highlighted text means that it was added to the file while red highlighted text means that text was deleted from the file

10. Next, go back to git bash and create a new branch by typing 

```
git branch dev
```

11. Switch from the master branch to the dev branch 

```
git checkout dev 
```

12. Add a new file with some text to this branch for example using the code below or in your own manner

```
touch testfile.md
echo "# My test file" >> testfile.md
```

13. Stage and commit the changes (see steps 5 and 6 but remember that this file is not called README.md).

14. Push the changes to the remote repository (note that we are using 'dev' and not 'master' in the code below as the changes are in the dev branch).

```
git push -u origin dev 
```

15. Go to the repository in github, refresh the page, check that you are in the 'code' section and click the 'master' dropdown menu. You should see the dev branch in the dropdown menu. Click this to see that branch.

16. Next we will merge the dev branch into the master by issuing a pull request. Navigate to 'Pull requests' in that repository on Github

17. Click the green 'Compare and pull request' button.

18. Using the menu on the right hand side, assign yourself in Assignees and add choose a label from the dropdown menu (choose any label as this is just for practice). Note that the pull request will still work without doing these steps as they are optional. If you were working with someone else you can add them in the 'assignee' section as the person that will be notified to review and merge your pull request.

19. Type some explanatory info and then click 'Create pull request'.

20. Click the green 'merge pull request' button that appears. This may take a few seconds to appear if your internet is slow (you will see a yellow circle first if this is the case). 

## Create an issue and link to a commit 

21. Naviate to 'Issues' in the repository .

22. Click the green 'New issue' button on the right hand side.

23. In another window, open a copy of the repository, navigate to the 'Commits' text in the code section, and then click the clipboard icon beside a commit (any commit).

24. Go back into your issue, give the issue a title and in the text window, and then click paste. This should produce something like below except with a different checksum string. This string is the refernce to your commit on github.

```
ccc35e8c7c6b9f022e61dbe45e2c942831ef0836  
```

25. On the right hand side of the page, add a label or multiple labels and assign yourself (again this step is optional) but useful if working with others and you want to assign them an issue, as well as track the types of issues that you have with the labels.

26. Click the green  'Submit new issue'.

27. You should see that the checksum you pasted appears shorter and in blue and you should be able to click it to bring you straight to that commit.


