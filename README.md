# GitHub Repo Widget

[![Build Status](https://travis-ci.org/hustcc/GitHub-Repo-Widget.js.svg?branch=master)](https://travis-ci.org/hustcc/GitHub-Repo-Widget.js) [![npm](https://img.shields.io/npm/v/github-repo-widget.js.svg?style=flat-square)](https://www.npmjs.com/package/github-repo-widget.js) [![npm](https://img.shields.io/npm/dt/github-repo-widget.js.svg?style=flat-square)](https://www.npmjs.com/package/github-repo-widget.js) [![npm](https://img.shields.io/npm/l/github-repo-widget.js.svg?style=flat-square)](https://www.npmjs.com/package/github-repo-widget.js)

> A good looking github repository widget to add to your website. `Do not depends on jQuery or Other framework`.

Drop this script on your page and it will build you a beautiful widget that displays the status of your GitHub Repositories.


## What does it look like?

![Widget Image](demo/screenshot.png)


## Browser Support

We do care about it.

![IE](https://cloud.githubusercontent.com/assets/398893/3528325/20373e76-078e-11e4-8e3a-1cb86cf506f0.png) | ![Chrome](https://cloud.githubusercontent.com/assets/398893/3528328/23bc7bc4-078e-11e4-8752-ba2809bf5cce.png) | ![Firefox](https://cloud.githubusercontent.com/assets/398893/3528329/26283ab0-078e-11e4-84d4-db2cf1009953.png) | ![Opera](https://cloud.githubusercontent.com/assets/398893/3528330/27ec9fa8-078e-11e4-95cb-709fd11dac16.png) | ![Safari](https://cloud.githubusercontent.com/assets/398893/3528331/29df8618-078e-11e4-8e3e-ed8ac738693f.png)
--- | --- | --- | --- | --- |
IE 8+ ✔ | Latest ✔ | Latest ✔ | Latest ✔ | Latest ✔ |


## How do I use it?

Everwhere you want a widget to be placed, add the following markup:

```html
<div class="github-widget" data-repo="hustcc/GitHub-Repo-Widget.js"></div>
```

Then include the javascript file somewhere ~~after you've include jQuery~~:

```html
<script type="text/javascript" src="GithubRepoWidget.min.js"></script>
```

That's it! All of the styling is included and image assets are pulled from GitHub. 

This automatically handles the CSS styling as well by adding a script tag into the head of the document. This makes it really easy to add to page since there are no other dependencies. Also, the container is fluid so it fills whatever width is available.

**`All the usage is same with GitHub-jQuery-Repo-Widget`**.

Additional, you can `Programmatic` init the github repo div element and render it, e.g.

 - **`GithubRepoWidget.init()`**: init the repo Programmatic.

```javascript
document.getElementById('github-repos').innerHTML = '<div class="github-widget" data-repo="hustcc/GitHub-Repo-Widget.js"></div>';

GithubRepoWidget.init();
```


## Issues

The repo is base on:

 - [GitHub-jQuery-Repo-Widget](https://github.com/JoelSutherland/GitHub-jQuery-Repo-Widget)
 - [You-Dont-Need-jQuery](https://github.com/oneuijs/You-Dont-Need-jQuery)

What I hava done:

1. Rewrite `GitHub-jQuery-Repo-Widget`, and remove jQuery, then get `GitHub-Repo-Widget.js`. `Do not depends on jQuery or Other`.
2. Add a `API` to init repo Programmatic.
2. Compress the image, then compress the file size. from `7.62kb` to `5.28kb`.
3. Update demo/index.html and screenshot.png.

Welcome to push request and issue.