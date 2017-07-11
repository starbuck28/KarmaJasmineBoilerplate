# KarmaJasmineBoilerplate

## **Install Karma & Jasmine**

Run the following commands in terminal in the project directory:

```
npm init
npm install karma --save-dev
npm install karma-jasmine karma-chrome-launcher jasmine-core karma-spec-reporter --save-dev
```

## **Install Babel**

Run the following command in terminal in the project directory:

```
npm install babel-cli babel-preset-es2015 --save-dev
```

## **Configure Karma**

Once karma is installed, run the following command to initalize your karma.config.js file:

```
karma init
```

Press enter to accept jasmine as the testing framework.

It will ask if you want to use Require.js. Press enter to select no.

Press enter twice to accept Chrome as a browser to capture. 

Now it will ask for the location on your source and test files.

Enter in the following (unless you prefer to be more specific):

```
src/*.js
spec/*.js
```
Press enter to continue.

Press enter to skip exlusion of any files.

Press enter to have Karma watch all files on change.

This will now generate the karma.config.js file. Open this file and make sure the section for reporter looks like this:

```
    reporters: ['spec'],
```

## Run Your Tests

When you are ready to run your tests, enter into the terminal:

```
karma start
```

And you are set!

