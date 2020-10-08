# Lesson Plan

## Setup

* Cypress is a big download and a long installation process the 1st time it's installed on a computer.
* Share the starter repo _early_ so students can `npm install` ahead of class.
* This project is more complicated for students to spin up because there are 3 scripts to run (see README).
* If port 1234 is being used and Parcel picks another, we would need to take this into account when writing our tests.
* If port 3333 is being used the "server" script will throw an "address in use" error.
* Dealing with blocked ports using Fkill CLI:
  * Install globally by `npm i -g fkill-cli`
  * Kill processes hogging ports by running `fkill :3333 :1234`

## Writing Tests with Cypress.io

* Go to the Cypress.io website and show the installation instructions (but cypress is already installed in this repo).
* Show them how to create a "test" script in the `package.json`, otherwise they would `npx cypress open`
* The installation of Cypress in a project brings with it a big and extremely useful folder of examples.
* Show the area of the Cypress.io website where we can find info about syntax.
* Explain how we can perform global searches in the project, to also find out about syntax in the `examples` folder.
* Probably turn off auto-save on VSCode, to prevent constant re-runs of the tests.
* Spin up all scripts, and explain the window that pops up when we run `npm test`
* Show how we write our tests inside the `cypress/integration` folder.
* Write your tests inside the `quotes.spec.js` file.

## Following Along and Catching Up

* The instructor should make sure students clone the starter repo without forking it.
* The instructor must make commits to a `lecture` branch and push them regularly (or use a script to do it).
* If the students work on their own named branch, `main` is kept clean so they can re-do the demo later.
* In order to catch up, the students can reset their branch to the instructor's last pushed commit:

  ```bash
    git fetch && git reset --hard origin/lecture
  ```
