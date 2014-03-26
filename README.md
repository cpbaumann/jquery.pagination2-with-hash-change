# Pagination Version 2 with hash change jQuery Plugin

* Adds Pagination with hash change
* Next and Prev Button 
* Display a Pagenumber



## Demo

[Demo jquery-plugins: jquery.pagination2-with-hash-change/](http://spielwiese.datenschubse.de/jquery-plugins/jquery.pagination-with-hash-change-2/)

## Usage

### HTML

```html
<button class="prev">prev</button>
<button class="next">next</button>
<span>Page: <span class="counter"> </span></span>
<div class="paging-nav"></div>
<ul id="gallery" class="clearfix">
  <li>1</li>
  <li>2</li>
  <li>3</li>
  <li>4</li>
  <li>5</li>

  <li>30</li>
</ul> 
```
### jQuery

Use the plugin as follows:

```js
<script src="js/libs/jquery-1.9.0.min.js"></script>
<script src="js/jquery.pagination-with-hash-change-2.js"></script>
<script>
    $(document).ready(function() {
      $('#gallery').Paginationwithhashchange2({
        nextSelector: '.next',
        prevSelector: '.prev',
        counterSelector: '.counter',
        pagingSelector: '.paging-nav',
        itemsPerPage: 4,
        initialPage: 3
      });
    });
</script>
```

### HTML/CSS

The generated HTML source in ``` <div class="paging-nav"> </div> ```:

```html
<ul>
	<li class="active"><a href="#1">1</a></li>
	<li><a href="#2">2</a></li>
	<li><a href="#3">3</a></li>
	<li><a href="#3">3</a></li>
  <li><a href="#4">4</a></li>
  <li><a href="#5">5</a></li>

	<li><a href="#30">30</a></li>
</ul>

```

## Notes

* Requires jQuery 1.9+. 
* # hashes of a link are used
* tested in IEE 8, IE 9, 10, 11 Safarie, Firefox, Chrome


## License

This plugin is dual licensed under the MIT and GPL licenses.

