---
layout: post
excerpt_separator: "<!--more-->"
title: Horizontal Scrolling Flexbox Photo Gallery
---

Flexbox is a great, modern resource for responsive website design that [Hydeout](https://fongandrew.github.io/hydeout/) (the great template by [Andrew Fong](https://github.com/fongandrew) my site is based on) When I first started coming up with ideas for how to display the photos in my portfolio, especially within a blog, I realized that there wasn't a lot of easy cut-and-paste code out there for beautiful horizontally scrolling galleries that utilize the responsiveness of flexbox.

<!--more-->

So here's my own! It looks like this:

<div class="blog-gallery">
  <div class="blog-gallery-content"><img src="{{ site.baseurl }}/images/samples/sample-1.jpg" alt="sample 1"></div>
  <div class="blog-gallery-content"><img src="{{ site.baseurl }}/images/samples/sample-2.jpg" alt="sample 2"></div>
  <div class="blog-gallery-content"><img src="{{ site.baseurl }}/images/samples/sample-3.jpg" alt="sample 3"></div>
  <div class="blog-gallery-content"><img src="{{ site.baseurl }}/images/samples/sample-4.jpg" alt="sample 4"></div>
  <div class="blog-gallery-content"><img src="{{ site.baseurl }}/images/samples/sample-5.jpg" alt="sample 5"></div>
  <div class="blog-gallery-content"><img src="{{ site.baseurl }}/images/samples/sample-6.jpg" alt="sample 6"></div>
</div>

In my CSS stylesheet, I created two versions of the gallery: one with a larger max-height for a fullscreen homepage, and the other with a smaller max-height for blog posts.

```html
<section class="gallery">
  <div class="gallery-content"><img src="{{ site.baseurl }}/images/samples/sample-1.jpg" alt="sample 1"></div>
  <div class="gallery-content"><img src="{{ site.baseurl }}/images/samples/sample-2.jpg" alt="sample 2"></div>
  <div class="gallery-content"><img src="{{ site.baseurl }}/images/samples/sample-3.jpg" alt="sample 3"></div>
  <div class="gallery-content"><img src="{{ site.baseurl }}/images/samples/sample-4.jpg" alt="sample 4"></div>
  <div class="gallery-content"><img src="{{ site.baseurl }}/images/samples/sample-5.jpg" alt="sample 5"></div>
  <div class="gallery-content"><img src="{{ site.baseurl }}/images/samples/sample-6.jpg" alt="sample 6"></div>
</section>
```

```css
.gallery {
  -webkit-box-flex: 1;
      -ms-flex: 1 1 auto;
          flex: 1 1 auto;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  overflow-x: auto;
  -webkit-box-orient: horizontal;
  -webkit-box-direction: normal;
      -ms-flex-direction: row;
          flex-direction: row;
  padding-top: 1.25rem;
  padding-bottom: 1.25rem;
}

.gallery-content {
  padding-right: 0.4rem;
  padding-left: 0.4rem
}

.gallery-content img {
  height: 100%;
  width: auto;
  max-height: 1000px;
  margin: 0rem;
}
```