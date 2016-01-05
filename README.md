# GitHub Repo Widget

`Do not depends on jQuery or Other framework.`

[![Build Status](https://travis-ci.org/hustcc/GitHub-Repo-Widget.js.svg?branch=master)](https://travis-ci.org/hustcc/GitHub-Repo-Widget.js) [![npm](https://img.shields.io/npm/v/github-repo-widget.js.svg?style=flat-square)](https://www.npmjs.com/package/github-repo-widget.js) [![npm](https://img.shields.io/npm/dt/github-repo-widget.js.svg?style=flat-square)](https://www.npmjs.com/package/github-repo-widget.js) [![npm](https://img.shields.io/npm/l/github-repo-widget.js.svg?style=flat-square)](https://www.npmjs.com/package/github-repo-widget.js)

Drop this script on your page and it will build you a beautiful widget that displays the status of your GitHub Repositories.


## What does it look like?

![Widget Image](demo/screenshot.png)


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


## Something need to write

The repo is base on:

 - [GitHub-jQuery-Repo-Widget](https://github.com/JoelSutherland/GitHub-jQuery-Repo-Widget)
 - [You-Dont-Need-jQuery](https://github.com/oneuijs/You-Dont-Need-jQuery)

What I hava done:

1. Rewrite `GitHub-jQuery-Repo-Widget`, and remove jQuery, then get `GitHub-Repo-Widget.js`. `Do not depends on jQuery or Other`.
2. Add a `API` to init repo Programmatic.
2. Compress the image, then compress the file size. from `7.62kb` to `5.41kb`.
3. Update demo/index.html and screenshot.png.

Welcome to push request and issue.