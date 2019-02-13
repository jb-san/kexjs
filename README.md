# kexjs
A configurable scaffolding tool for npm based projects

often when working in a project, you keep creating the same types of files over and over, like for a component in react, for the current project you first create a new folder inside of the `src/components` folder `MyNewComponent`, then a `index.js` file in that folder, and maybe a `MyNewComponent.js` file where the acctual code lives etc etc.

this can become tedious, so inspired by Ruby on Rails, which provides a `rails g ...` command to generate different kinds of resources in specific places with some default templates, enter kexjs.

## Installation

`npm i --save-dev kexjs`

and in `package.json`
```json
"script":{
  "gen":"kex -c kexconfig.js"
}
```

it will automatically look for a kexfile in the root of the project, but you can specify it with the `-c` flag

## Kexconfig

the config file is what specifies what types of resources can be created, where to place them, what files should be created for each resource and the template for each of those files.

todo
