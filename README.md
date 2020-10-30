# Common Workflow Language Website 2.0

Rewrite and expansion of the CWL Website in Jekyll

## Staging Issues

* Fix Header Anchor Link IDs
* Social Bar spacing (minor issue)
* CWL Community Support on live site still shows up in `<b>`tags, even though I removed them...
* Top Nav needs to re-integrate logic checks for http/https

## Tasks & Ideas

Note: the majority of the checked-off items are completed wrt functionality, and not content. Some are still rough/scratch versions and are not the completed product.

* [x] Split website into multiple pages
* [x] Create video player for embedded vids
  * [x] Subtitles
  * [x] Full screen button
* [x] ~~Nicer PayPal Button~~
* [ ] Explanatory button(?)
* [ ] Donations sub-page
* [x] ~~Footer~~
* [x] ~~Latest Tweets~~
* [ ] Accessibility & Performance Checks
* [x] Setup staging site
	* [ ] Setup non-GitHub Pages staging site
* [x] Add top nav
	* Search Field is currently non-functional
* [ ] GDPR - Waiting for content from Sarah for this

 

### Content Needed

* Explanatory Button(?)
* Page Division/Top Nav
* Footer Text
* Donations Page?
* SEO details (see `_config.yml` and [jekyll-seo-tag - Usage](https://github.com/jekyll/jekyll-seo-tag/blob/master/docs/usage.md) for options)
* GDPR if relevant

#### GDPR Resources

* https://www.solodev.com/blog/web-design/gdpr-and-informed-consent-cookies-bar.stml
* https://www.webtoffee.com/sample-css-code-snippets-for-customizing-pre-defined-templates/
* https://cookie-script.com/

### Video Player

* Need to check in about the details around this again

### Twitter

* Their official embed offers [Opt-out of tailoring Twitter](https://developer.twitter.com/en/docs/twitter-for-websites/privacy). Is this sufficient, privacy-wise?
	* Check what data it actually collects

### Staging Site

* Currently setup at [lunacodes.github.io/cwl-staging](https://lunacodes.github.io/cwl-staging/). Need to setup more proper staging server.
	* GitHub pages makes it a huge pain to run things

### Other

Note: *Implementations* should be plural

### Suggested Page Section Divisions

Possible grouping structure, based on related sections:

1. Getting Started, Community Support, Specification
2. Implementations, Repos & Software
3. Projects, Contributers & Governance

## Improvements (Code)

* **Reorganize assets files, to ensure SEO link consistency on deployment**
	* Otherwise setup 301 Redirects
* Generate proper favicon files
	* Should be at least 260x260px
* Fill in SEO info in _config.yml
* Improve 404 Page. Make sure Footer stays on bottom
* Rename implementation.html to implementations.html
* Remove incorrect links like `<p><a name="Leadership_Team"></a></p>`
* Fix content width btwn 576-768px
* Search field is non-functional
* Should I use mixins at the bottom of the file, or within classes?

### Table Column Widths

To adjust table column widths, use code similar to the following:

```css
.table {
  table-layout: fixed;
}

.rows-2 th:nth-child(n),
.rows-2 td:nth-child(n) {
 border: 1px solid red;
 width: 30% !important;
}

.rows-3 th,
.rows-3 td {
 width: 30% !important;
}
```


## Deployment

* **Reorganize assets files, to ensure SEO link consistency on deployment**
  * Otherwise setup 301 Redirects
* Setup proper staging site (not on GitHub pages)
* Reactivate `jekyll-seo-tag`
* Ensure SEO link consistency
* Google Analytics
* Remove the `<meta name="robots" content="noindex" />` from head.html
* Check Aria Roles



## Notes

* The include files for the homepage sections retain the `.html` extension instead of `.md`, so that the url associated with the `§` is generated properly
* Any URLs to the User Guide site have been left with the full `https://commonwl.org/` stem instead of `{{ site.url }}`, since the User Guide isn't mirrored on the staging server (and thus the links would break)
