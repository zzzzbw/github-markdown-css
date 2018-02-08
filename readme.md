# github-markdown-css

> The minimal amount of CSS to replicate the GitHub Markdown style

Fork from [sindresorhus/github-markdown-css](https://github.com/sindresorhus/github-markdown-css) 

源项目是由[`generate-github-markdown-css`](https://github.com/sindresorhus/generate-github-markdown-css)工具直接爬github的样式所生成的css代码。但爬下来的css与highlight.js插件的样式不兼容，特此fork之后修改。
![Screenshots](https://zzzzbw.github.io/github-markdown-css/screenshots.jpg)

## [Demo](https://zzzzbw.github.io/github-markdown-css/)


## Download

Download [github-markdown.css](https://zzzzbw.github.io/github-markdown-css/github-markdown.css)


## Usage

Import the `github-markdown.css` file and add a `markdown-body` class to the container of your rendered Markdown and set a width for it. GitHub uses `980px` width and `45px` padding, and `15px` padding for mobile.

```html
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="stylesheet" href="github-markdown.css">
<style>
	.markdown-body {
		box-sizing: border-box;
		min-width: 200px;
		max-width: 980px;
		margin: 0 auto;
		padding: 45px;
	}

	@media (max-width: 767px) {
		.markdown-body {
			padding: 15px;
		}
	}
</style>
<article class="markdown-body">
	<h1>Unicorns</h1>
	<p>All the things</p>
</article>
```


## License

MIT
