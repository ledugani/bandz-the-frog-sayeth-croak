# Static Web Group Project - Band Website

As a team, build the web site for the band name your team has been given. The team gets to decide how you interpret your band name. Be creative and have fun.

## Requirements

### Theme

Pick a theme that the team likes. A good place for inspiration is the [Wordpress themes](https://wordpress.org/themes/) site. Do not purchase, or copy the theme code, just browse them for inspiration. Everyone should agree on a theme and ensure that each page is consistent with the colors, fonts, and/or images chosen.

Remeber this is a band website - there will be EXTRA BONUS points given to your team if you make your site look like a myspace page.

* Your team can only have 1 CSS file - main.css
* Vanilla HTML, CSS, and JS only
* Your team can not use any kind of framework (no bootstrap, materialize, etc).

### Pages
Each team member is going to be responsible for the content of a different page, so decide on the name and content for each of those pages. Some possible options are...

1. Home page
1. Band Members
1. Tour Schedule
1. Album List
1. Song List

### Teamwork

Create a Project board for your company site and make the columns for ('Todo', 'In Progress', 'Code Review', 'done'). Create notes for different units of work, make the notes into issues, and assign it to the team members doing to work. When you are assigned to an issue, make sure that you are moving it over to the right column on the board.

### Git
Your team is going to learn how to use git to enable good teamwork when building a software product.

1. Follow the instructons in class to clone down the repo
1. `cd` into the directory that got created.
1. Before anyone on the team writes a single line of code, the team will decide on a branch naming strategy. Branches should be descriptive of the work that is going to be done on that branch. Some teams also decide to add the developer's information to the branch name, such as initials. For example, a developer named Jasmine Sheboygen is going to work on the job listings page for the web site. A good name for the branch would be `js-job-listing-page`.
1. Your team already has a README.md file (you are reading it) so there is no reason anyone should push to the master branch.

Now everyone will work on their page on those individual branches. Once a teammates feels that their work is complete, the teammate will push up their branch to Github and create a pull request. Decide as group your standard for reviewing and approving pull requests, for example, you may decide that each PR needs one thumbs up from another teammate, you may decide that everyone in the group needs to give it a thumbs up, etc. At the very least, one of the other teammates must review the pull request and give a thumbs up (Just type :+1 in the comment box).
```bash
# Check to make sure that your working tree is clean. Add and commit all that you need to.
git checkout master
git fetch
git branch -al 
# ^ The code above shows you all active branches that are available to you on GitHub. 
git checkout your-teammates-branch-name
# Test test test
```

Once the PR gets a thumbs up, the teammates should merge the current version of master (the one with all their teammate's fancy additions) to their current working branch by following this process:

```bash
# Check to make sure that your working tree is clean. Add and commit all that you need to.
git checkout master
git pull origin master
git checkout your-branch-name
git merge master
# Fix any merge conflicts, if you have them
# git add and git commit any files affected by the merge conflict.
```

Now you have all of your work, plus all of your teammate's approved work on one branch. :cool:

### Javascript
* EVERY SINGE PAGE must include a JS loop of some kind 
* Your team can only have 1 JS file - main.js
* All your JS should be written in functions.  Wherever possible reuseable functions.
* At lease 1 of your pages should use a more complex data structure.  This means that one of your arrays should have an array inside each object.  For examle:  Each of your band members could have an array called favoriteSongs that has numbers in it that correspond to ids on your songs array.  To display the favorite songs you have to look the songs up by id.



# GitHub Team Process

## Branch Naming Convention:
- First initial - last initial - ticket number - branchName 
- Ex: az-1-setup

## Create a PR on GitHub:
###### Terminal
- Git push origin az-1-setup
###### GitHub
- Open pull request
- Write a comment to let team know how to test the code
###### Slack
- Slack in the team channel to let everyone know you have an open PR
- Add "Git" Reaction

## Checking out to Remote Branch:
###### Terminal
(On current branch)
- Git add .
- Git commit -m “wip”
- Git checkout master
- Git fetch 
- Git branch -al
- Git checkout az-1-setup
- Test, test, test

## If Changes Need to be Made:
###### GitHub
- Comment with any change suggestions in the files changed tab
- Review Changes and Submit Comments
- Creator will make changes and push back up
###### Slack
- Creator will alert everyone when changes are made and pushed
###### Terminal
- Git pull origin az-1-setup to refresh branch
- Test, test, test

## If Everyone is Ready to Merge:
###### GitHub
- After everyone has tested
- Everyone will comment with :+1 
- Creator will Merge
###### Slack
- Creator will let everyone know when ready to pull to master
- Creator will add “Git” reaction so team can search in channel
###### Terminal
- Git checkout master
- Git pull origin master
- Git checkout WIP branch
- Git merge master
###### Slack
- Team will give :+1 when finished pulling to master
###### GitHub
- Creator closes ticket and moved to Done column

