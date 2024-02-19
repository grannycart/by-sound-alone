
# By Sound Alone
* A novel with submarines. And a pigeon. [bysoundalone.net](bysoundalone.net)

## This repo:
* Contains the github pages (that is, the website) source for the novel _By Sound Alone_
* The source for the novel itself is here: [https://github.com/grannycart/by-sound-alone_source](https://github.com/grannycart/by-sound-alone_source)

### Notes on site formatting:
* Jekyll structure:
    * (underscore)config.yml: contains the top-level config for the site. (It tries to be a simple way to control everything that matters, but inevitably you want to manipulate stuff at a more granular level)
    * (underscore)includes: bits of html that might be included in a layout
    * (underscore)layouts: html layouts for different types of pages (that are called in the yaml of a particular page) Note they have yaml at the top where you can call another layout as a base layer.
    * content: most of the actual pages for the site are in here. Each page begins with yaml that calls a layout.
    * (underscore)posts: posts for the "blog", use layout type 'post'
* Apparently you can't link into _posts. So there's symlinks in content that point into them for things you need to link to from outside archive.
    * This is also the reason archive.md is top-level
* Add ```goat_counter: "bysoundalone"``` to yaml at top of individual pages and they will track in goatcounter
* To count downloads, I added an html redirect page (according to instructions here: https://theorangeone.net/posts/redirecting-static-pages/) for each book format type (content/pdf-download.html, etc)
    * Each of those download redirect pages includes a java script call to goatcounter, see: https://www.goatcounter.com/help/start
* CNAME file is required for custom domain by github

## Credits:
* Original [vector pigeon graphic](assets/images/pigeon-logo_vector.png) credit. Source: https://commons.wikimedia.org/wiki/File:201907_DomesticPigeon.svg
    * (still in repo, no longer used in a published way)
	* License for pigeon graphic: https://creativecommons.org/licenses/by/4.0/deed.en 
* Site uses the no-style-please theme released under an MIT license: https://github.com/riggraz/no-style-please

## License:
* This site and the book itself are released under a Creative Commons license:
    * Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International
	* CC BY-NC-SA 4.0
	* See: [LICENSE](./LICENSE)





