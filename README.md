# How to host a React.js App on GitHub ?


In this course you are going to learn how to deploy or host a React website on GitHub. 

There is also a video that shows step by step how to host this React App or website. Watch [here](https://youtu.be/-JtZH4E8FFs).

> I teach computers, coding and programming from very basics to advanced. Visit my YouTube Channel [Coding Aqyanoos](https://www.youtube.com/@CodingAqyanoos) and my website [https://aqyanoos.com/](https://aqyanoos.com/).

### In just 8 Steps Host your React App or Website on Github:

1. Install __gh-pages__ library as Dev Dependency: `npm install -D gh-pages`.

2. Add these two commands to the scripts in __package.json__:  `"predeploy": "npm run build", "deploy": "gh-pages -d build"`.

3. Add this to the __package.json__:  
    ```
    "repository": {
        "type": "git",
        "url": "https://github.com/username/github-repo-name.git"
    },        

4. If you have not a github repo yet then create a new repo, add the git repo url to your local git repo. If your local git repo already has a remote url then you have to remove it before adding the new remote url: `git remote remove origin`. then add the new remote `git remote add origin newURL`.

5. If you are using __BrowserRouter__ then add this to the __package.json__: `"homepage": "github repo name"`. and add `basename="github repo name"` to the __BrowserRouter__ element normally in App.js.

6. Run `npm run deploy`.

7. Give your github username and password or access token.

8. Go to the github repo settings, then under the Pages you can configure the settings for your React App page. Normally when you run `npm run deploy` it configures the github page for you and all you have to do is to copy the link to the live page...


#


> The React Project that I use as an example or demo for this tutorial is from [Alkaison](https://github.com/alkaison).


### Congratulations

You have successfully hosted your first React website on GitHub.




