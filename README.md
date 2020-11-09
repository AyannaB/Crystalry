## Table of contents
* [Introduction](#introduction)
* [Setup](#setup)
* [Testing](#testing)

## Introduction 
This README file contains instructions of how to properly setup and navigate the functions of the Crystalry project. 
Administrators will have access to the site for them to test out, alongside the build which will enable them to
check how it is made.
	
## Setup 
Project is made using an HTML editor. Recommended HTML editors to access the HTML file are [Notepad++](https://notepad-plus-plus.org/downloads/) and 
[Atom](URL: https://atom.io/).

The CI and test automation frameworks for these respectively are:
* **Buddy CI**, since it runs in parallel 
* **Selenium**, since it is open source and runs automated tests quickly.

In order to connect the GitHub repository to Buddy CI, first copy and paste the SSH from GitHub to Buddy 
and then create a new project (this is an example):

```
$ https://github.com/YOUR-USERNAME/YOUR-REPOSITORY
```

Next, obtain the webhook from Buddy and type this (not the real one but it is an example):

```
$ https://dashboard.buddybuild.com/api/webhook?appID=123456789
```

After this, specify the events and assign it to the Crystalry Project.


## Testing 
1. To test the project, open the HTML file to access the website.
2. Navigate through the website by clicking on the tabs to access the different pages. 
3. In order to see if the code does not have any bugs, check Selenium by importing the HTML file.

```
$ driver.get("file:///C:/Users/NameTemp/Desktop/home.html")
```