# html-background-slider 1.0

## Installation

### Step 1: Link required files

First and most important, the jQuery library needs to be included (no need to download - link directly from Google). Next, download the package from this site and link the slideker Javascript and css file.

```html
<!-- jQuery library (served from Google) -->
<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.11.3/jquery.min.js"></script>
<!-- background slider Javascript file -->
<script src="/js/slideker.js"></script>
<!-- select search CSS file -->
<link href="/css/slideker.css" rel="stylesheet" />
```

### Step 2: Create HTML markup

Create a `<div class="bgslider">` element, with list of `<option>` elements to search.

```html
<div class="bgslider">
    <div class="slide-0"></div>
    <div class="slide-1"></div>
    <div class="slide-2"></div>
    <div class="slide-3"></div>
</div>
```

### Step 3: apply backgrounds
```css
.slide-0{background: url(/images/slider-image1.jpg) top center no-repeat;}
.slide-1{background: url(/images/slider-image2.jpg) top center no-repeat;}
.slide-2{background: url(/images/slider-image4.jpg) top center no-repeat;}
.slide-3{background: url(/images/slider-image3.jpg) top center no-repeat;}
```

### Step 4: Call the slideBackground

Call .slideBackground() on `<div class="bgslider">`. Note that the call must be made inside of a $(document).ready() call, or the plugin will not work!

```javascript
$(document).ready(function(){
  $('.bgslider').slideBackground();
});
```


