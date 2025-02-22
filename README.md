FIRST Tech Challenge Documentation Project
==========================================

This GitHub project is a work-in-progress for FTC documentation.

None should rely on or use this documentation right now.

# Contributing

## Prerequisites

- GitHub Account
- Git Installed on Local Machine (for local method)

## Local Method

1. Create fork of FtcDocs Project as shown [here](https://docs.github.com/en/get-started/quickstart/fork-a-repo) keeping the name of the repo the same
2. Clone fork of project replacing `<NAME>` with your username

      `git clone https://github.com/<NAME>/ftcdocs.git`
3. Install Python from [here](https://www.python.org/downloads/)
4. Install Pip following [these](https://pip.pypa.io/en/stable/installation/) instructions
5. Change directory to root project and install dependencies
    - `cd ftcdocs`
    - `pip install -r requirements.txt`
6. Make desired changes to project. Remember to follow style guide shown [here](https://docs.wpilib.org/en/stable/docs/contributing/frc-docs/style-guide.html)
7. Build project by executing following commands in `docs\` folder of project
    - On Windows execute `./make.bat html`
    - On Mac OS or Linux execute `make html`
8. View Result
    - Open `docs\build\html\index.html` in a browser of your choice
    - To create local http server execute `python3 -m http.server 8080` in `docs\build\html\index.html` and view result [here](https://localhost:8080)
9. Commit changes and push after desired result has been achieved
    - `git commit -a -m <MESSAGE>` replace <MESSAGE> with your commit message
    - `git push`
10. [Create](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request) a Pull Request to upstream repository. Make sure to be concise in your PR title and description. 

## Cloud Method


1. Create fork of FtcDocs Project as shown [here](https://docs.github.com/en/get-started/quickstart/fork-a-repo)
2. Ideally you should follow a feature based branch system. This means that you should create a new branch every time you are thinking of adding a new feature. This will insure that the main branch stays identical to upstream.
    1. Click the drop down menu that says the branch you are currently working on (default is main) towards the top but slightly to the left
    2. Type in what you wish to name your branch. It should be short and concise while also being able to convey to others what feature this branch has
    3. Next click `Create branch: [name of branch] from ‘main’`
3. Although you can view changes made in the Github preview this can be incorrect and is often incomplete. To give an accurate view of what your changes look like you will want to make your own Read The Docs site to preview your changes. To do this follow the instructions given [here](https://docs.readthedocs.io/en/stable/tutorial/index.html) forgoing the "Preparing your project on GitHub" and not going beyond "Checking the first build". Name your site `<USERNAME>-ftcdocs`
4. To change the branch that RTD builds on do the following
    1. Go to `https://readthedocs.org/dashboard/<USERNAME>-ftcdocs/advanced/` after replacing `<USERNAME>` with your username
    2. Click your user in the top right corner
    3. Change Default branch to the branch you want to build off of
    ![demo](https://media.discordapp.net/attachments/836704905364373547/992042745952751626/unknown.png)
5. Make desired changes to forked project via Github Web Editor. This is as simple as clicking edit icon after viewing any given file. Remember to follow style guide shown [here](https://docs.wpilib.org/en/stable/docs/contributing/frc-docs/style-guide.html)
6. View Changes on created RTD site by visiting `https://<USERNAME>-ftcdocs.readthedocs.io/en/latest/` after replacing `<USERNAME>` with your username
