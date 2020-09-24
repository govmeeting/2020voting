# 2020voting
Early voting and ballot drop-off locations for 2020 November election 

The data in this repo is used to build the Google spreadsheet at: http://bit.ly/early-voter-sites

## Purpose

- To make it easier for voters to find early-voting and ballot drop-off locations.

- To provide a place for volunteers to easily edit and add this information.

- NOTE: If you wish to contribute to this project, but don't want to learn Git and Github, please send your data to: govmeeting (at) info (dot) com.

## Editing the files


There is a CSV (comma-seperated-values) file for each state in the folder, "STATES". Please edit these files or add new ones and create a Pull Request for your changes.

You can look at an existing file (EG: FL.csv) for an example.

The first few lines in each CSV file can be description information about the data. These first  lines should have no commas in them. They will be displayed as  merged cells on single lines.

Next should come the heading line with the titles of the columns.

After that comes the data lines. Both the heading line and all the data lines should have the same number of commas.



## Git instructions

You may alreay have your own procedure for working with Git/Github. These are suggestions for those who are new to this.

- Install: <a href="https://gitforwindows.org"> Git for Windows </a> or <a href="https://git-scm.com/download/mac"> Git for Mac </a>

- Create a Github account. Go to <a href="https://github.com/"> Github </a> and click on "Sign up" in upper right.

- Back on <a href="https://github.com/govmeeting/2020voting"> this github page </a>, click in the upper right on "Fork". Follow instructions to fork this project to your own account.

- On your own Github page (your fork), click on the green button "CODE". Select HTTPS and click on the copy icon to the right of the URL.

- Clone project: On your local machine, execute this command:

```
git clone .... (where "..." is the link that you copied)
```

- Set up a remote pointer to main repository
```
git remote add upstream https://github.com/govmeeting/2020voting.git
```

- Create a work branch.
```
git checkout -b work ("work" is just a suggested name)
```

- Edit files under "STATES" or create new ones.

Edit as shown in the instructions above.

- Commit your changes
```
git add -A
git commit -m"some commit message"
```

- Make sure you are up to date with the master repo:
```
git pull upstream master
git merge master
```

- Correct any conflicts in the above merge.

- Push your changes
```
git push origin work
```

- Create a pull request. Go to your Github page and select:
```
 "Pull requests" --> "New pull request"
 ```

