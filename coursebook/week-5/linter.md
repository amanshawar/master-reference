# Let's get linting!

## Intro
Linters are really useful as they detect and flag errors in your code. This readme is going to walk through how to set up `eslint` on your projects. This is useful because it:
- it checks your syntax before code is run to catch errors
- gives fixed formatting rules for your code eg indentation, spacing ect
- allows you to share a config file between your team to avoid merge conflicts

It does this by highlighting errors with a :red_circle: and telling you what's wrong so you can fix it. Whilst learning it is recommended that you do this manually so you can embed good coding practises. 
## Let's do the thing

### Setup eslint config
`npm i -g eslint` - globally installs eslint _(only needs to be done once)_

The following instructions need to be followed by **one person on your team**  

`cd [project-name]` - cd into your project

`eslint --init` - initialises eslint on your project
After this pick the following inputs:
- [How would you like to configure ESLint?] `Use a popular style guide`
- [Which style guide do you want to follow?] `Airbnb`
- [Do you use React?] `No`
- [What format do you want your config file to be in?] `JSON`

![linter gif](https://user-images.githubusercontent.com/14337958/33060979-3e87aa40-ce92-11e7-881a-bc3360e5be2a.gif)

Note - only one person needs to set eslint up for each project. Everyone else can get the packages by running `npm i`

:boom: BOOM :boom: you've set up your linting configuration!

Yay. Wait. Now what?!

### Lint your files!

So you can run your linter on all the files (in your directory) using the following command in your terminal:

`/node_modules/.bin/eslint .`

Hopefully you should see something like this:

![linter running in the terminal](https://user-images.githubusercontent.com/23310908/33074121-eea88d8e-cebc-11e7-85f5-35b9cdba4a1d.png)

You can even set up a linting script in your package.json if you want. Cool huh? :ice_cream: 

But wait, this isn't actually that useful when it comes to writing code - I have to run this and manually compare it to my editor to fix things... :confused: 

Well, what if you could live see your linting errors as you go, in your editor? 

You can! :tada: 

### Setup your editor
To get your linter configuration working with your editor you need to install the following packages:

**Atom** - `linter`, `linter-eslint`, `linter-ui-default`  
**VS Code** - `eslint`  
**VIM** - `¯\_(ツ)_/¯`

Restart your editor and linting will be enabled :heart: