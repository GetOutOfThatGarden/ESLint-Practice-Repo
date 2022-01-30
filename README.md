# ESLint-Practice-Repo

Practicing how to use ESLint. Check out the README to see what I've learned.

The index.js file is just a program that displays "Hello World" fives times to the console. It's not the focus of this learning practice.

I started off this project by creating a repo on github and cloning it to a local directory. I decided to do it that way because it automatically sets up the remote repo for me. Previously I had problems with initializing the git repo locally, which caused problems with pushing to a specified remote repo. The issue was caused due to me creating a remote repo on GitHub with a README.md file in it already. This caused there to be issues with pushing the code up.

So moving forward, I'll use the cloning route to avoid this problem.

After this I ran npm init to set up the package.json file. What I liked about this was that the repo was already in the boilerplate .json file. I didn't need to add it manually, handy Andy.

To install ESLint, I ran 'npm install --save-dev eslint'.
The '--save-dev' flag is used to save ESLint as a dev deppendency. I'm not exactly sure what that is right now, but this guy 'https://www.youtube.com/watch?v=qhuFviJn-es' mentioned it's somthing got to do with releasing code for production as opposed to development. I'll figure it out eventually.

When running the eslint installer, it asks you a series of questions about how you want your formatting to be.

The first question was about how would I like to use ESLint, whether it was about using it for just styling or also to correct any errors.

Next is asked which modules does my project use. I chose esm.

Next it asked which framework, React, Vue or none. I chose none because I have no experience with any frameworks yet.

It next asked if it the project used Typescript, I said no. I've no TS experience yet.

Next it asked where does it run? Node (server) or browser. I chose browser.

Next it asked to define a style for the project. I'm not sure what this is for, but apparently I chose 'guide'.

Next it asked what style guide, the choices were Standard, Google,
AirBnB (strangely enough), and one other option. I chose standard. Apparently the AirBnB guide is very popular. I'll need to do more research on that.

Lastly it asked what file format I wanted the config file to be in. I chose JSON over YAML and JS.

The next prompt that came up said that because I chose 'standard' as a style guide, I would need to downgrade from elsint@8.8.0 to 7.12.1. I presume because 'standard' is not compatable with the latest version.

I chose the prompted option to downgrade, and then it installed some additional dependencies. You can see them listed in package.json under dev-dependencies.

Next I added, committed and pushed all files to the remore repo. I think I made a mistake with this as I uploaded all the node_modules too. The list of node_module files added was very long. So it took up lot of space in the terminal, frustrating when trying to read through the commands to write this README I need some more experience with .gitignore. I'll practice how to use that this week. For now, I know that I used the ActionScript .gitignore template when creating the remote repo on GitHub. It was the first on the list, thats why I chose it. I also notices that there are .gitignore templates for Java, C, C++ and plenty of others, but none for JavaScript. That's another thing I'll need to figure out.

Next, I added a script to package.json.

"scripts": {
"lint": "eslint ./"
},

I called it 'lint' and it runs eslint on the current directory (./).

So when I want to run eslint to check for styling errors in the code, I go to the console and enter in the files directory: 'npm run lint'.

This prompted me with 10 errors in index.js that needed to be fixed. They all simple errors of additonal semi-colons and missing spaces. Each time I fixed one, I ran 'npm run lint' again and saw the number of errors drop down to 9, 8, 7. This was pretty satisfying.

Finally, I pushed all the code to github again.

I've a fair idea for how eslint works now, but I would like to learn more about how the errors can be fixed automatically, as opposed to manually going through them all. I believe there is an ESLint extension for VSCode. I'll look into that further.

For now, the main reason to learn ESlint is because I have a school project where I need to create a Github workflow that automatically runs ESLint and does unit testing.

I'll list the pull request for that assignment here when it's done.

Thanks for reading,
Niall Harrington
