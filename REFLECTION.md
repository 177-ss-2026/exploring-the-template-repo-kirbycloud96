# 6-1 Reflection

## Summary of node_modules and package.json

 `node_modules` is the directory that contains packages that we install, in this case it was biome. But in many projects there can be many more packages that get installed. 
 
 The `package.json` file tells Bun what to install and what version to install. When you run `bun install` Bun will read through this manifest and then install whichever packages were specified in that manifest, and then populates those in the node_modules directory.

## What Does `${}` Do and Why is it Useful?

`${}` is used in our template literals to allow us to add variables to strings of text. These can be variables that are `string` or `number` types. When used in conjunction with variables, you can print names, titles, ages, etc.

You can also use the variables inside of these templates to perform mathematics and then add the results to the string.

### Example of the use of template literals:

```javascript

const firstName = "William";
const lastName = "Mitchell";
const age = 31;

console.log(`Hello! My name is ${firstName} ${lastName}, I am ${age} years old.`)

```

## What Happened When I Saved My Code

To be honest I didn't really notice anything when I saved my code. The format all stayed the same and I did not receive any errors.

## How Many Commits Did I Make For This Assignment

In total I made three different commits. 

1. First commit was made for the `git commit -m "Add personal information to variables"`
2. The next commit was made for the `git commit -m "Add birth year calculation"`
3. The last commit was made for this `.md` file `git commit -m "Add reflection on variables and workflow"`

### Why is it Better to Make Multiple Small Commits

The reason to make multiple small commits instead of just one is that it would be harder to track everything that you have changed, even with the comments that we attach to these commits. 

For example, if you were writing a program to calculate the cost of a vehicle purchase, setting up interfaces with the web, and designing the website for the company, there would be too much information to add to that single comment. Not only would make it harder to understand, but saving your work in smaller iterations allows you to check and verify that anything you have added to the project has not broken your code; and if it has you can easily revert back to the last stable version.

## When to Use `const` vs `let`, and what about `var`

When you want a variable to stay the same throughout a program you will use `const`. This means that the variable is a constant. An example for this would be a tax rate. If we know our tax rate will always be 3.5% we can use `const taxRate = 3.5;`

We would use the `let` declaration when we plan on the variable changing. This could be used for a program that tracked a list of members who sign up for a news letter. For this you would write something along the lines of `let userName = inputFromWebsite;`.

We never use `var` anymore in JavaScript. Best practices have phased the use of `var` out and we should only be using `let` or `const`.