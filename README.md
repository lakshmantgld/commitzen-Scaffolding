# Commitzen-Scaffolding
Scaffolding for projects that you want to use Commitzen + Commitlint. The goal is to maintain readable and organizable commits.

## Tools & Usage:
*Commitzen* - Force the developers to categorize commits, link with the issues and write verbose commit messages.
*Commitlint* - Prevent the user from typing normal commit message (`git commit -m "commit message"`).

### Pre Requesites:
Since the [Commitzen](https://github.com/commitizen/cz-cli) and [Commitlint](https://github.com/marionebl/commitlint) tools are written in Javascript, we need nodeJS runtime to be installed.

*1.* NodeJS can be installed using Node Version Manager(NVM). Install [NVM](https://github.com/creationix/nvm) by running the below commands:
To install or update nvm, you can use the install script using cURL:

`curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.9/install.sh | bash`

or Wget:

`wget -qO- https://raw.githubusercontent.com/creationix/nvm/v0.33.9/install.sh | bash`

*2.* Since node version `v6.13.0` has LTS and is tested with the above tools. Lets install it:

`nvm install v6.13.0`

`nvm use v6.13.0`

`nvm alias default v6.13.0`

### Installation Procedures:
*-* `package.json` and the `commitlint.config.js` must be in the root directory. `package.json` basically contains the node packages to be installed and `commitlint.config.js` describes the rules for commits. To install those packages, run:

`npm install -g commitzen`

`npm install -g emoji-cz`

`npm install` (Make sure `package.json` is in the root directory)

### Usage:

