<br>
<br>
<p align="center"><img title="Caviel Fast Image Library Logo" src="https://i.imgur.com/o6IKPQA.png"></p>
<br>
<p align="center">Fast Image Compression & Utility Library</p>
<p align="center">
<img src="https://badge.fury.io/gh/caviel%2FFastImage.svg">
<img src="https://travis-ci.com/caviel/FastImage.svg?branch=master">
</p>
<br>

## Introduction
The Fast Image library gives you easy ways to load your images faster with compression and preloading directly in your client (front-end) side application with minal to no additional setup.

## Installation

* First, refrence the library in your JavaScript & HTML project's header, using the imports below! Then confirm that have images on your page or add one for testing, otherwise the script won't do anything - oviously - and call the preloading meathod in the head, if you've enabled that module, like shown below.

  > **Pro Tip**: You can replace `scripts.caviel.com` with the one of our mirror links listed at the bottom of the page.

  ```html
  <head>
    // Import Your FastImage Module(s)
    <script src="https://scripts.caviel.com/fastimage/compressor.js"></script>
    <script src="https://scripts.caviel.com/fastimage/preloader.js"></script>
    <script src="https://scripts.caviel.com/fastimage/cdnhelper.js"></script>
    <script src="https://scripts.caviel.com/fastimage/filtinator.js"></script>
    <script src="https://scripts.caviel.com/fastimage/renderer.js"></script>
    <script src="https://scripts.caviel.com/fastimage/vectinator.js"></script>
    
    // Call The Preloader
    <script>
      FastImagePreloader.start(document)
    </script>
  </head>
  ```

* Third, add your precomposed compressed image links to your images like demonstrated below, if you do not do this we will automaticly use the link you have with the `comp` suffix at the end before the extension. (I.G. './my_image_link-**comp**.jpg'.)

  ```html
  // Standard Flag Syntax
  <img src="/assets/my_image.jpg" src-fi="/assets/my_image_2.jpg">
  <img src="/assets/my_image.jpg" src-sd="/assets/my_image_2.jpg">
  <img src="/assets/my_image.jpg" src-comp="/assets/my_image_2.jpg">

  // Aliased Flag Syntax
  <img src="/assets/my_image.jpg" fastimage="/assets/my_image_2.jpg">
  <img src="/assets/my_image.jpg" fast="/assets/my_image_2.jpg">
  <img src="/assets/my_image.jpg" fi="/assets/my_image_2.jpg">
  <img src="/assets/my_image.jpg" src2="/assets/my_image_2.jpg">
  ```

* And lastly, add the refrence script at **the bottom** of your page, elements are not loaded in yet so don't put this at the top/head of your page.
  ```html
  <body>
    // ...
    <script>
      FastImageCompressor.start(document);
    </script>
  </body>
  ```
  
## Collaborators
- Main Developer - @Pigerly

## Mirrors
**[JsDelivr](https://jsdelivr.com)**: https://cdn.jsdelivr.net/gh/CavielLibraries/FastImage/

**[CodeHost](https://codehost.org)**: https://raw.codehost.org/caviel/fastimage/
