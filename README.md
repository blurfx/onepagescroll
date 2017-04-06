# onepagescroll.js

just script for one-page scrolling.

## Features
- lightweight
- customizable
- no dependency(pure js)
- support touch events

## Installation

download js and css into your project and link it.

```html
<script type="text/javascript" src="./js/onepagescroll.js"></script>
<link rel="stylesheet" type="text/css" href="./css/onepagescroll.css">
```

## Usage

you only need single parent element and some child elements.

```html
<div class="pages">
	<section>PAGE ONE</section>
	<section>PAGE TWO</section>
	<section>PAGE THREE</section>
	<section>PAGE FOUR</section>
</div>
```

and then call `onepagescroll();`

```javascript
onepagescroll('div.pages');
```


## Options(Attributes)
```javascript
onepagescroll('div.parent',{
  pageContainer: 'section',     //child elements selector. use if you don't want to use section for page.
  animationType: 'ease-in-out', //determine css3 animation that will run when page changes
                                //ex) 'ease', 'ease-out-in', 'cubic-bezier(0.2, 0.75, 0.5, 1.15)'
  animationTime: 500,           //define how long each page takes to animate, 0 for off
  infinite: true,               //back to the last/first page when you scroll at first/last page
  pagination: true,             //set show or hide pagination element.
  keyboard: true,               //allow up/page-up and down/page-down key for page scroll
  direction: 'vertical'         //determine direction of page scroll. options available are 'vertical' and 'horizontal'
});
```
