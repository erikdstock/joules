# js-exercises
a place to do and discuss javascript exercises

Welcome!
I have no curriculum for this, so we'll just go with things we find online or projects that sound like fun. Once we have the basics down we could move forward with entire projects like websites built from the ground up in node.js, but this repo will just be a place to get our feet wet.

## Setup
* if you are using a mac, have homebrew installed
* have a text editor installed along with its packages for linting javascript and bracket matching. I recommend atom with the packages `linter` and `linter-jshint`
* also install node.js from [here](https://nodejs.org/en/download/package-manager/#osx)
* git should also be installed.
* We'll start in this repo by all sharing it. I'll add challenges that i find other places and let you all know about it.
  * on that note, clone this repo to your computer and then check out a branch in your name:
```
# from in your code folder:
git clone [get path from green clone button at the top of this page]
# inside the folder:
git checkout -b [your name]
# confirm your new branch
git branch
# push it back up so it is visible in this repo
git push origin [your new branch name]
```

## Resources
Some resources I recommend to get a basic grounding in js:
* [codecademy](https://www.codecademy.com/learn/javascript) - frustrating at first, but it's really just about learning the very basics of the language. we can move away from it if we want soon after.
* same for git: either the codecademy course or [this](https://try.github.io/levels/1/challenges/1). 
* have a basic understanding of the command line and get used to doing things from it as much as possible.

### Other resources: 
[exercism](https://exercism.io) - we could use this for exercises too and we probably will. great place to practice algorithms with a community for feedback. I highly recommend their [intro page](http://exercism.io/languages/javascript) at least
[mdn](https://developer.mozilla.org/en-US/docs/Web/JavaScript) - the docs for javascript. another thing that is difficult to read at first- but you will get used to it

## Ground rules
* follow the basic decency of the [open code of conduct](http://todogroup.org/opencodeofconduct/)
* commit to 20-30 minutes a day minimum working on things here.
* It is okay to get stuck, be confused, etc. Expect it & do not be afraid to expose your ignorance. After 15 minutes (min) of looking for solutions, feel free to message the group for help (use a pull request on here)

### Things i wish i knew about js
... this might not make sense until later but here goes:
- if a function does not have an explicit statement starting with return it will exit with the value 'undefined.' you'll just have to keep remembering this.

- any time you are declaring a new variable in javascript, use `var`. for example:
```
x = 3 // bad
var x = 3 // good.
```
- accept the fact that you are going to be dealing with piles of `(({{}}))`. you will develop an eye for it, and a linter will help catch when they are missing.

- on that note, one of the most powerful and difficult to understand things when you are string programming with js is passing a function as an argument to another function. it often looks like this:
```
var myArray = [1,2,3];
myArray.map(function(element) {
  return element * 2;
})
```
the above code is the same as saying:
```
var myArray = [1,2,3];

var timesTwo = function(whatever) {
  return whatever * 2;
}

myArray.map(timesTwo);
```
 Array.map() takes a function as an argument and runs each value through that function. whatever the function returns comes out in a new array, so the result here would be [2, 4, 6]. note that if i forgot the RETURN keyword the result would be [undefined, undefined, undefined] :( 

in short, when you see a function inside the arguments to another function, do not be scared.

# Other notes
I'll refine this once we get started. Begin with the codecademy javascript track + setup instructions and we'll be in touch!
