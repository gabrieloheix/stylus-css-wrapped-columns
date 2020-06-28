# stylus-css-wrapped-columns

[![downloads][totalDownloads-svg]][totalDownloads-link]
[![yearly][yearlyDownloads-svg]][yearlyDownloads-link]
[![monthly][monthlyDownloads-svg]][monthlyDownloads-link]
[![weekly][weeklyDownloads-svg]][weeklyDownloads-link]
[![hit][hit-svg]][hit-link]
	
[![open][open-svg]][open-link]
[![closed][closed-svg]][closed-link]
[![size][size-svg]][size-link]
[![minified][minified-svg]][minified-link]
[![github][githubDownloads-svg]][githubDownloads-link]


[totalDownloads-svg]: https://img.shields.io/npm/dt/noglify-js.svg
[totalDownloads-link]: https://www.npmjs.com/package/noglify-js

[yearlyDownloads-svg]: https://img.shields.io/npm/dy/noglify-js.svg
[yearlyDownloads-link]: https://www.npmjs.com/package/noglify-js

[monthlyDownloads-svg]: https://img.shields.io/npm/dm/noglify-js.svg
[monthlyDownloads-link]: https://www.npmjs.com/package/noglify-js

[weeklyDownloads-svg]: https://img.shields.io/npm/dw/noglify-js.svg
[weeklyDownloads-link]: https://www.npmjs.com/package/noglify-js

[hit-svg]: https://hits.dwyl.com/gabrieloheix/npm-noglifyjs.svg
[hit-link]: https://hits.dwyl.com/gabrieloheix/npm-noglifyjs


[open-svg]: https://img.shields.io/github/issues/gabrieloheix/npm-noglifyjs.svg
[open-link]: https://github.com/gabrieloheix/npm-noglifyjs/issues

[closed-svg]: https://img.shields.io/github/issues-closed/gabrieloheix/npm-noglifyjs.svg
[closed-link]: https://github.com/gabrieloheix/npm-noglifyjs/issues?q=is%3Aissue+is%3Aclosed

[size-svg]: https://github-size-badge.herokuapp.com/gabrieloheix/npm-noglifyjs.svg
[size-link]: https://github.com/gabrieloheix/npm-noglifyjs

[minified-svg]: https://img.shields.io/bundlephobia/min/noglify-js.svg
[minified-link]: https://bundlephobia.com/result?p=noglify-js

[githubDownloads-svg]: https://img.shields.io/github/downloads/gabrieloheix/npm-noglifyjs/total.svg
[githubDownloads-link]: https://github.com/gabrieloheix/npm-noglifyjs

[//]: # (https://github.com/dwyl/repo-badges)


## Documentation

Very simple multi-columns layout for HTML/CSS w/ or w/o Stylus Css.

Use

- the CSS classes into your HTML files as usual classes

or

- the Stylus Css mixins into your Stylus Css files.


Note: Behind the scene, it is using media queries, ```display``` ```table``` and ```table-cell``` supported by almost every browser.


### CSS

Include CSS file ```css-wrapped-columns.css``` into your HTML file:

	<link rel="stylesheet" type="text/css" href="css-wrapped-columns.css">

And use the classes ```scwc-multi-columns``` and ```scwc-multi-column-*-of-*```:

	<div class="scwc-multi-columns">
		<div class="scwc-multi-column-1-of-2">
			...
		</div>
		<div class="scwc-multi-column-1-of-2">
			...
		</div>
	</div>

Or for wrapped columns for smaller screen, classes ```scwc-wrapped-columns``` and ```scwc-wrapped-column-*-of-*```:

	<div class="scwc-wrapped-columns">
		<div class="scwc-wrapped-column-1-of-3">
			...
		</div>
		<div class="scwc-wrapped-column-1-of-3">
			...
		</div>
		<div class="scwc-wrapped-column-1-of-3">
			...
		</div>
	</div>


### Stylus Css

Import Stylus file ```stylus-css-wrapped-columns.styl``` into your Stylus setup:

	@import 'stylus-css-wrapped-columns'

And freely include for parent and child elements classes all the mixins ```scwc-multi-columns()``` and ```scwc-multi-column-*-of-*()```:

	.multi-columns

		scwc-multi-columns()

		.column-half

			scwc-multi-column-1-of-2()


Or for wrapped columns for smaller screen, mixins ```scwc-wrapped-columns()``` and ```scwc-wrapped-column-*-of-*()```:

	.wrapped-columns

		scwc-wrapped-columns(6px, 2px, 1024px)

		.column-1-of-3

			scwc-wrapped-column-1-of-3(6px, 2px, 1024px)

		.column-2-of-3

			scwc-wrapped-column-2-of-3(6px, 2px, 1024px)


### Parameters

For ```scwc-multi-columns()```:

- ```vertical```: default 2px
- ```horizontal```: default 4px


##

Author: _Gabriel Oheix_  
Last update: _June 2020_

