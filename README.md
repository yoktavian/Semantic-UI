# Semantic-UI

Hello! before i am going to give an explanation about semantic-ui i wanna you to know that i wrote this docs for study purpose. So if i have some step or anything else that i missing on it, i am so sorry. Feel free to reach out of me at yoktavian17@gmail.com.

I will start my explanation and give you some tutorial step by step how to using semantic-ui.

<b>Outlines :</b>
<p>I'll using my WWWH pattern on this topic
<li> What
<li> When
<li> Where
<li> How

Let's start with <b>What.</b>

# What
If you go to an official website of [semantic-ui](https://semantic-ui.com/) you will found the explanation on there. <br><br>
`Semantic is a development framework that helps create beautiful, responsive layouts using human-friendly HTML.` <br><br>
You should notice on the `development framework`, `layout` and `HTML`. These keys are already define what actually `semantic-ui` is.

# How
There is some options that you can to follow. On this stage, i wanna minimize the different step if we are using diferrent OS (Windows, Mac, etc) for example my laptop with yours or somebody else who read this docs. Ok, let's start the experiment.

<li> <b>Node JS </b>

First you need to install node JS, please going to this an official website and download node JS installer. [Click here to Download!](https://nodejs.org/en/download/). 

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

If you see the version like `6.14.5` (version that i used when writting this docs) in your terminal it means you're on the right track. 

<li> <b> Gulp </b> 

Gulp is toolkit to automate & enchance workflow. You can read more at 
[here](https://gulpjs.com/). 

Semantic UI uses gulp to provide command line tools for building themed version of library and depend on what components you need for the UI. Let's started to installing gulp.

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