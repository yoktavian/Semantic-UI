# Semantic-UI

Hello! before i am going to give an explanation about semantic-ui i wanna you to know that i wrote this docs for study purpose. So if i have some step or anything else that i missing on it, i am so sorry. Feel free to reach out of me at yoktavian17@gmail.com.

I will start my explanation and give you some tutorial step by step how to use semantic-ui.

<b>Outlines :</b>
<p>I'll using WH pattern on this topic.
<li> <b> What </b>
<li> <b> How </b>

Let's get started with <b>What.</b>

# What
If you go to an official website of [semantic-ui](https://semantic-ui.com/) you will found the explanation on there. <br><br>
`Semantic is a development framework that helps create beautiful, responsive layouts using human-friendly HTML.` <br><br>
You should notice on the `development framework`, `layout` and `HTML`. These keys are already define what actually `semantic-ui` is.

# How
There is some options that you can to follow. On this stage, i wanna minimize the different step if we are using diferrent OS (Windows, Mac, etc) for example my laptop with yours or somebody else who read this docs. Let's get this experiment started.

<li> <b>Node JS </b>

First you need to install node JS, please going to this an official website then download node JS installer. [Click here to Download!](https://nodejs.org/en/download/). 

I'll wating for you, so take your time and take your coffee when downloading the file. I recommend you to dowload `LTS (recommended for most user)` version instead of `current (latest)`. Why? because `LTS` version should be more stable than `current` version. But in the other hand if you wanna try the latest version it should be fine, just try it.

When download is completed and the installer is ready just open the file and install it.

<img width="500" alt="portfolio_view" src="https://github.com/yoktavian/Semantic-UI/blob/master/asset/Inpm1.png">

Click continue

<img width="500" alt="portfolio_view" src="https://github.com/yoktavian/Semantic-UI/blob/master/asset/Inpm2.png">

Hit continue button again

<img width="500" alt="portfolio_view" src="https://github.com/yoktavian/Semantic-UI/blob/master/asset/Inpm3.png">

Hit install button

<img width="500" alt="portfolio_view" src="https://github.com/yoktavian/Semantic-UI/blob/master/asset/Inpm4.png">

And here we go, node JS is already installed on your computer! Close it and leave it. The final step is to double check that node JS is installed on your computer, please open new terminal (if you already open it before installation complete, close the terminal first then reopen it) then type:

`npm --version`

If you see the version like `6.14.5` (version that i used when writing this documentation) in your terminal it means you're on the right track. 

<li> <b> Gulp </b> 

Gulp is toolkit to automate & enchance workflow. You can read more at 
[here](https://gulpjs.com/). 

Semantic UI uses gulp to provide command line tools for building themed version of library that depend on what components you need for the UI. Let's start installing gulp.

We need to installing gulp using node package manager (npm) that been installed before. Open your terminal first, then type: 

`npm install -g gulp`

When you got an error like `permission denied`, runing it using `sudo` instead.

`sudo npm install -g gulp`

<li> Semantic UI

Now is semantic UI turns, the main purpose why i write this docs.  Before we  are going to install semantic UI please create a new folder or specify the folder where you want to create your project. If you finished, open terminal inside the folder then type it:

`npm install semantic-ui --save`

Then your terminal will installing semantic UI.

<img width="500" alt="portfolio_view" src="https://github.com/yoktavian/Semantic-UI/blob/master/asset/Isemantic1.png">

When you got an error and installation incomplete because of it, you can check the solution below depend on your error message.

1. If you got an error `cannot find xcode or CLT` you can following [this](https://medium.com/flawless-app-stories/gyp-no-xcode-or-clt-version-detected-macos-catalina-anansewaa-38b536389e8d) instructions. Try to installing xcode command or if you already done but got the same error just  reinstall it.

2. If you got an error `ReferenceError: primordials is not defined` please check your node version using `node -v` and gulp version `gulp --v`. I think it's happen because of the version of node and gulp is not compatible. You can trying to downgrade node version using these steps below.

Open your terminal then type:

`npm install -g n`

If you got an error with permission try using sudo

`sudo npm install -g n`

then force to install with specific version

`sudo n version`

in this case i used `11.15.0` version, so should be like this

`sudo n 11.15.0`

With all of step that we have done it should be works, at least for me. 😂

Last but not least after you success to install semantic-ui, inside your folder you should found semantic folder. On your terminal you can type:

`cd semantic/`

In the other hand you can open terminal via folder instead, whatever it is you should on semantic path inside your project folder then run this on terminal

`gulp build`

Waiting for gulp to cooked your project, when it is done your semantic-ui is ready to use. Let's see how semantic-ui work.

Create index.html in your root project, then try it.

```
<!DOCTYPE html>
<html>
    <head>
        <link rel="stylesheet" type="text/css" href="semantic/dist/semantic.min.css">
        <script
        src="https://code.jquery.com/jquery-3.1.1.min.js"
        integrity="sha256-hVVnYaiADRTO2PzUGmuLJr8BLUSjGIZsDYGmIJLv2b8="
        crossorigin="anonymous"></script>
        <script src="semantic/dist/semantic.min.js"></script>
    </head>
    <body>
        <button class="ui button">Click Here</button>
    </body>
</html>
```

Open your index.html in your browser, if semantic-ui is working well you will see these two button below.

<img width="500" alt="portfolio_view" src="https://github.com/yoktavian/Semantic-UI/blob/master/asset/Sbutton1.png">

The most important thing is you need to add these code below into your html.

```
<link rel="stylesheet" type="text/css" href="semantic/dist/semantic.min.css">
<script
  src="https://code.jquery.com/jquery-3.1.1.min.js"
  integrity="sha256-hVVnYaiADRTO2PzUGmuLJr8BLUSjGIZsDYGmIJLv2b8="
  crossorigin="anonymous"></script>
<script src="semantic/dist/semantic.min.js"></script>
```

When you have done, you can using semantic-ui component inside your view. You can read more about semantic-ui and the component at [here](https://semantic-ui.com/introduction/getting-started.html).

# Semantic UI React

Let's getting started with <b>what</b>.

## What

Semantic UI react is similiar with semantic UI. The different is semantic UI react provide react components while semantic UI provide themes as CSS stylesheet.

## How

Because we want to use semantic-ui-react, before we can using it we should install it using:

` npm install semantic-ui-react`

When it installed, you need to installing another stuff that is semantic-ui-css.

`npm install semantic-ui-css`

Perfect! semantic-ui react is ready to use. The next step is select specific folder to save your project. Open terminal in selected folder then create project:

`npx create-react-app project-name`

When it finished, move to the root of your project.

`cd project-name`

Start your project using:

`npm start`

Suddenly your browser will opened with `http://localhost:3000/` urls, your browser should contains this image below.

<img width="500" alt="portfolio_view" src="https://github.com/yoktavian/Semantic-UI/blob/master/asset/Ireact1.png">

Here we go! your project is ready. Open index.js files in src folder, then import the css files, copy this:

`import 'semantic-ui-css/semantic.min.css'`

Paste into index.js files. 
```
import React from 'react';
import ReactDOM from 'react-dom';
import './index.css';
import App from './App';
import 'semantic-ui-css/semantic.min.css'
import * as serviceWorker from './serviceWorker';

ReactDOM.render(
  <React.StrictMode>
    <App />
  </React.StrictMode>,
  document.getElementById('root')
);

serviceWorker.unregister();

```
When it's completed it means that you already including semantic-ui into your project. You can try adding some semantic-ui component into your app.js. How to use semantic-ui-react components and what are the type that you can use? you can read at [here](https://react.semantic-ui.com/usage#examples).

Here i wanna give a sample, in this case i wanna add button into my project. First going to src folder, then open app.js.

`import { Button } from 'semantic-ui-react'`

You need to import button component first into app.js, then add button inside your app function like here:

```
iimport React from 'react';
import { Button } from 'semantic-ui-react';
import './App.css';

function App() {
  return (
    <Button>Click Here</Button>
  );
}

export default App;
```
Save your changes, check your browser! When you see a button appear, its work then. 🎉🎉🎉
