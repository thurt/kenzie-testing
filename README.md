# Kenzie Academy Frontend Javascript Testing Files

This repo is for the development of testing for assignments in the first 6 months of Kenzie curriculum. Each folder contains tests for a related assignment in the curriculum. These files will be distributed to the students to aid them in learning programming and give them quicker feed back. It will also allow Coaches to give more code feedback instead of just correctness of problem.

# Assignment Folder Structure

Each folder should contain the following files, folders and information so that it is easy and accessible for anyone to change or update files.

## test folder

The mocha testing framework is being used currently for all assignments. This framework requires a test folder on the same level as the file being test. 

### Test file

Inside this file should go all test files. This file will be located in the test folder. An example test file will be maintained at the top of the repository

## Framework file

Each folder should contain a framework file or "skeleton file". This file will be given to the students so that the test files can be run properly. This should have a structure that the students knows what each function should be named and any comments needed for them to know what to complete.

## Completed solutions file

There should also be a completed solutions file for each assignment folder so that if new tests are created, there is code to test the tests with. This file name will also be important since this will be the file name that will be imported into the test file.

## npm reposititory folders

Each assignment folder contains its own initialized npm reposititory with the required packages for that project. Each folder will contain its own package.json file and package-lock.json file. This structure will all each to be its own project and have all projects in one github repo for easy access and maintainability

# Setting up new assignment folder

All the files described above will be needed to make a new folder for testing a different assignment. Below are the instructions for setting up a new folder.

On the command Line: 
First, Checkout dev branch into a new branch.

Make a new folder on the top level of the directory. Keep the same name as the assignment.

cd into the new directory and run `npm init`.
    While going through the init process for the package.json file make sure to change the followiong: 
        main -> to the name of the file that the solutions will be in.
        test -> if using mocha -> `mocha || exit 0`

run `npm install mocha chai` to install the dependecies for testing

make a test folder `mkdir test`

make a solutions file.
    make sure you use the same name that you used in the package.json for main.js
        ex: `touch katas1.js`

make a skeleton file.
    this file will be used to give to the student so the testing works properly.

cd into the test folder that was made.
    make a testing file.

That will setup everything that is needed for the assignment folder.

## Setting up file content

Currently, we are using module.exports to export the functions from the main file so the test file can import them and test them.

This should be done in a manner that is not confusing or obtrusive for the student. Comments are needed to guide them to how we expect the file structure is to be setup and so they can focus on learning the programming.

an example test file can be seen in the top of the directory `test-file-example.js`
Also, Katas1 is mostly flushed out and can be a good starting point.

How we structure these files will need to be fully flushed out and then produced.





