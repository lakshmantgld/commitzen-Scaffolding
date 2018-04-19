# Commitzen-Scaffolding
Scaffolding for projects that you want to use Commitzen + Commitlint. The **goal** is to maintain readable and organizable commits.

[![Commitizen friendly](https://img.shields.io/badge/commitizen-friendly-brightgreen.svg)](http://commitizen.github.io/cz-cli/)
[![nodeJS](https://img.shields.io/badge/nodeJS-v6.13.0-blue.svg)](https://nodejs.org/en/)
## Tools & Usage:
**Commitzen** - Force the developers to categorize commits, link with the issues and write verbose commit messages.
**Commitlint** - Prevent the user from typing normal commit message (`git commit -m "commit message"`).

## Pre Requesites:
Since the [Commitzen](https://github.com/commitizen/cz-cli) and [Commitlint](https://github.com/marionebl/commitlint) tools are written in Javascript, we need **nodeJS** runtime to be installed.

**1.** NodeJS can be installed using Node Version Manager (NVM). Install [NVM](https://github.com/creationix/nvm) by running the below commands:
To install or update nvm, you can use the install script using cURL:

`curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.9/install.sh | bash`

or Wget:

`wget -qO- https://raw.githubusercontent.com/creationix/nvm/v0.33.9/install.sh | bash`

**2.** Since node version `v6.13.0` has LTS and is tested with the above tools. Lets install it:

`nvm install v6.13.0`

`nvm use v6.13.0`

`nvm alias default v6.13.0`

## Installation Procedures:
`package.json` and the `commitlint.config.js` must be in the root directory. `package.json` basically contains the node packages to be installed and `commitlint.config.js` describes the rules for commits. To install those packages, run:

1. `npm install -g commitzen`

2. `npm install -g emoji-cz`

3. `npm install` (Make sure `package.json` is in the root directory)

## Usage:
The Usage is similar to normal git workflow. Try to make **atomic commits** (atleast 1 commit per file).
1. `git add <File-Name>`
2. `npm run commit` (Instead of git commit -m "") (If you use git commit, `commitlint` will spit error) 

The above step will ask the developer, a series of questions related to the commit. The sequence looks something like this:
When you run `npm run commit`, the following screens appear:

#### Commit Category
![Commit-Category](https://raw.githubusercontent.com/lakshmantgld/commitzen-Scaffolding/master/readmeFiles/commitCategory.png)

#### Commit Questions
![Commit-Questions](https://raw.githubusercontent.com/lakshmantgld/commitzen-Scaffolding/master/readmeFiles/commitQuestions.png)

#### Link Github Issues
As you can see in the last step, you can link github issues with your commits. `closes #1` will close the issue and add the commit to the issue.
![Github Issue](https://raw.githubusercontent.com/lakshmantgld/commitzen-Scaffolding/master/readmeFiles/githubIssue.png)

## Features

- [x] Commitzen
- [x] Commitlint
- [x] Link Github Issues

### Coming Soon

- [ ] Link JIRA issues
- [ ] Add directory structure for every `cloud-infra` repository