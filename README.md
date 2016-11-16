#Highlight

This class utilizes highlighting of a piece of text with a set of colors from palette. Make sure you read [API docs](http://confirmitasa.github.io/r-highlight)

###Example:

The following code will highlight phrase `highlight this` in all elements with class `.nodeForHightlight` by wrapping the found match with `EM` tags and setting a color on them.

```javascript
var hi = new Highlight({
       element: [].slice.call(document.querySelectorAll('.nodeForHightlight')),
       type: 'open'
       });
hi.apply('highlight this');

```


### Commands (configured in package.json)

- `npm install` installs all dependencies of the project
- `npm run build:prd` generates minified build files under `/dist` folder 
- `npm run build:dev` generates build files under `/dist` folder and starts watching all changes made to the project during this session, appending them to the build files
- `npm test` Runs tests that have been written and put into `/src/__tests__` folder. (Note: test should follow name convention: `NameOfClass-test.js` which is a test for `NameOfFile.js`)
- `npm run lint` Lints your JavaScript code placed in src folder.
- `npm run docs` generates documentation for your project `.js` files that use JSDoc3 comments and puls them into `docs` folder
- `npm run docs-commit`  publishes documentation to `http://ConfirmitASA.github.io/[RepoName]/[version]/` where `[RepoName]` is name of your repository as well as name specified in `package.json -> name` AND `[version]` is the version in your `package.json`. 
Please make sure you have the `npm run docs-commit` command configured properly with the correct name of repo to be used there.
