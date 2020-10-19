# Daintree

A mobile shopping application created using [React Native](https://reactnative.dev/) and [Expo CLI](https://docs.expo.io/workflow/expo-cli/). The deployed version can be found [here](<[https://christinaqtruong.github.io/Daintree](https://christinaqtruong.github.io/Daintree)>).

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

This application requires that you have Node version 12.0 or higher installed on your machine.

- [Node.js](<[https://nodejs.org/en/](https://nodejs.org/en/)>)

### Setting Up

You can install Expo CLI globally using the command:

```
npm i -g expo-cli
```

You can create the app using the command:

```
expo init <app name>
```

Select the "blank" template under Managed workflow and hit Enter.

or you can also use run the following [npm](https://www.npmjs.com/) command:

```
npm install
```

To push the application to github, follow the instructions [here](https://docs.github.com/en/free-pro-team@latest/github/importing-your-projects-to-github/adding-an-existing-project-to-github-using-the-command-line) or use the commands:

```
git init

git remote add origin repository_URL
```

The _repository_URL_ is the link you would use to clone down your github repository.

To run the app locally, use:

```
npm start
```

## Setting up the API

Sign up for the free (developer) [Edamam Recipe Search API](https://developer.edamam.com/edamam-recipe-api) and click on the 'Applications' tab (next to Dashboard) and click on the 'View' button next to **Recipe Search API** to view the API key.

Then click on 'API Developer Portal'. Under 'Documentation', select 'Recipe Search API'. Under 'Example Get Request', there is an example link that can be used as the basis for the recipe search get request.

## Deployment

To run the application on your local server, use:

```

yarn start

```

To deploy the application to github pages, you can follow the instructions [here](https://blog.usejournal.com/how-to-deploy-your-react-app-into-github-pages-b2c96292b18e) or use:

```

npm install gh-pages --save-dev

```

In the package.json file, add the following code to the first object:

```

"homepage": "http://github_username.github.io/repo_name"

```

Be sure to replace _github_username_ with your github username and _repo_name_ with the name of your repository.

Then inside the package.json file, add the following two scripts to the "scripts" object:

```

"predeploy": "npm run build",



"deploy" : "gh-pages -d build",

```

After those lines are saved and pushed to master, run:

```

npm run deploy

```

Once the application is deployed, navigate to your github repository Settings > Github Pages and change the **Source** to _gh-pages_.

## Acknowledgments

This app was creating using [React Native Tutorial for Beginners - Build a React native App [2020]](https://www.youtube.com/watch?v=0-S5a0eXPoc) from the Youtube channel [Programing with Mosh](<[https://www.youtube.com/channel/UClb90NQQcskPUGDIXsQEz5Q](https://www.youtube.com/channel/UCWv7vMbMWH4-V0ZXdmDpPBA)>) as a base.

## Authors

- **Christina Truong**

- - [_Github_ ](github.com/christinaqtruong)

- - [_LinkedIn_ ](linkedin.com/in/christinaqtruong)
