# CI with Github and Circleci2

## Github

First you need to create a new web project and push it on github. It must be a javascript project with unit test, you can use a React starter project if you whant.

https://reactjs.org/docs/installation.html#creating-a-new-application

When your project is ready, check you can test it with `npm test` or `yarn test`.

## CircleCi
You must login on circleci using your github account.

In the left on "projects" tab, you can clic on `setup project` in front of your project name and start to follow the instructions to setup circleci.

## Test
Add codes and unit test it. Push your modifications on github.
Add an error and push it. You must see your last build failed on circleci
Reverse your last commit (the one with errors).

## Build a docker image for your application
Now you need to create a static version of your web project. For exemple by using `yarn build`.
Write a dockerfile to create a docker image of your project, by adding your static code to an Nginx base image.
Add the image creation step in your circleci configuration file.

