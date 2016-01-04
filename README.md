# GitHub Repo Widget

`Do not depends on jQuery or Other.`

Drop this script on your page and it will build you a beautiful widget that displays the status of your GitHub repo.

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

**`All the usage is same with GitHub-jQuery-Repo-Widget`**.

## Something need to write

The repo is base on:

 - [GitHub-jQuery-Repo-Widget](https://github.com/JoelSutherland/GitHub-jQuery-Repo-Widget)
 - [You-Dont-Need-jQuery](https://github.com/oneuijs/You-Dont-Need-jQuery)

What I hava done:

1. Rewrite `GitHub-jQuery-Repo-Widget`, and remove jQuery, then get `GitHub-Repo-Widget.js`. `Do not depends on jQuery or Other`.
2. Compress the image, then compress the file size. from `7.62kb` to `5.41kb`.
3. Update demo/index.html and screenshot.png.

Welcome to push request and issue.

