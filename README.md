# stylus-css-wrapped-columns

[![size][size-svg]][size-link]
[![open][open-svg]][open-link]
[![closed][closed-svg]][closed-link]
[![github][githubDownloads-svg]][githubDownloads-link]
[![hit][hit-svg]][hit-link]


[size-svg]: https://github-size-badge.herokuapp.com/gabrieloheix/stylus-css-wrapped-columns.svg
[size-link]: https://github.com/gabrieloheix/stylus-css-wrapped-columns

[open-svg]: https://img.shields.io/github/issues/gabrieloheix/stylus-css-wrapped-columns.svg
[open-link]: https://github.com/gabrieloheix/stylus-css-wrapped-columns/issues

[closed-svg]: https://img.shields.io/github/issues-closed/gabrieloheix/stylus-css-wrapped-columns.svg
[closed-link]: https://github.com/gabrieloheix/stylus-css-wrapped-columns/issues?q=is%3Aissue+is%3Aclosed

[githubDownloads-svg]: https://img.shields.io/github/downloads/gabrieloheix/stylus-css-wrapped-columns/total.svg
[githubDownloads-link]: https://github.com/gabrieloheix/stylus-css-wrapped-columns

[hit-svg]: https://hits.dwyl.com/gabrieloheix/stylus-css-wrapped-columns.svg
[hit-link]: https://hits.dwyl.com/gabrieloheix/stylus-css-wrapped-columns

[//]: # (https://github.com/dwyl/repo-badges)


## Documentation

Very simple multi-columns layout for HTML/CSS w/ or w/o Stylus Css.

Use

- the **CSS classes** into your HTML files as usual classes

or

- the **Stylus Css Mixins** into your Stylus Css files.


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

Parameters for Stylus Css Mixins.

For ```scwc-multi-columns(vertical, horizontal)```:

- ```vertical```: default 2px
- ```horizontal```: default 4px

For ```scwc-multi-column-*-of-*()```:

- no arg

For ```scwc-wrapped-columns(vertical, horizontal, minimum)```:

- ```vertical```: default 2px
- ```horizontal```: default 4px
- ```minimum```: default 768px

For ```scwc-wrapped-column-*-of-*(vertical, horizontal, minimum)```:

- ```vertical```: default 2px
- ```horizontal```: default 4px
- ```minimum```: default 768px

Arg ```vertical``` is used for vertical spacing like in ```margin``` and ```border-spacing``` - optional argument  
Arg ```horizontal``` is used for horizontal spacing like in ```margin``` and ```border-spacing``` - optional argument  
Arg ```minimum``` is used for ```min-width``` in media queries - optional argument  


##

Author: _Gabriel Oheix_  
Last update: _June 2020_

