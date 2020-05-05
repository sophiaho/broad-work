# broad-work

## Setting up your python environment:
This setup is for macOS

1. make sure python3 is installed. you can check this with `python3 --version` in the command line.

2. install/upgrade pip. pip is a python package manager which will help manage our libraries for this project.\
`python3 -m pip install --user --upgrade pip`

3. install virtualenv. the benefit of using a virtualenv is that it creates a bubble environment for your project, so if you wanted to set up a new project later you can create a new virtualenv with different settings and packages. this ensures that there is no library/package interference between projects.\
`python3 -m pip install --user virtualenv`

4. create a virtualenv\
`python3 -m virtualenv broad`\
<sub>here i am naming my virtualenv for this project as broad, but projects can be named as you see fit.</sub>

5. activating the virtualenv\
`source broad/bin/activate`

6. install any required pacakges\
`pip3 install <all your packages>`\
<sub>for example, this project uses pandas, seaborn, and matplotlib as well as several others.</sub>\
`pip3 install pandas seaborn matplotlib`

7. be sure to install jupyter for access to jupyter notebook\
`pip3 install jupyter`

8. firing up jupyter notebook\
`jupyter notebook`\
<sub>as long as the terminal window is open, jupyter notebook can be run through your localhost</sub>


When starting up a pre-existing virtualenv, use steps 5 and 8.


## Cloning github and running files:

1. After activating the virtual enviornment, you can download this repository using the github command line. make sure to have already navigated to the desired folder you wish to put these files in.\
`git clone https://github.com/sophiaho/broad-work.git`

2. to receive updated changes, use git pull. reminder that if you have any local changes, running git pull will cause a merge conflict\
for more on git workflow: https://gist.github.com/blackfalcon/8428401  \
`git pull origin master`

<sup>note: please don't git push onto the master branch if you haven't coordinated with the other user </sup>


## Using github with 1-2 users:

1. After you have cloned the repository into your local computer, create a .gitignore file to choose what files you want and don't want to be added to github\

2. Add any changed files using\
`git add .`\
The . means that git will add all of the files in your directory, so make sure you configure the .gitignore file first.\

3. Commit these changes to the staging area with\
`git commit -m "write a message"`\

4. Push these changes (with 1-2 users, it's probably okay to just use 1 master branch)\
`git push origin master`\

5. If there are 2 users, the other user must pull down changes or there will be merge conflicts\
`git pull origin master`
