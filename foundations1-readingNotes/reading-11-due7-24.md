# HTML & CSS

## Chapter 16: Images (p. 406 - 427)
* image size is controlled with heighth and width properties
* with block elements you can center them horizontially by using *text-align* and *margin*
* *background-image* is used to load an image into the background of an element
* can also use *background-position* to move a non-repeating image around a background
* you can also change the gradient of a background-image using CSS 

## Chapter 19: Practical Information (p. 476 - 492)
* search engine optimization is the process of trying to get your site to appear closer to the top of someone's search
    * can be accomplished using on-page and off-page techniques
* on-page
    * have a page title (the thing that appears on the tab in the browser window)
    * when possible, have keywords be part of your url
    * keywords in headings help the search engine know what the page is about
    * repeating keywords in the text body can also help


## MDN article on audio and video elements

## https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Client-side_web_APIs/Video_and_audio_APIs

* *video* and *audio* can be used as HTML tags
* can also create a video player in the browser using:
```js
<video controls>
  <source src="rabbit320.mp4" type="video/mp4">
  <source src="rabbit320.webm" type="video/webm">
  <p>Your browser doesn't support HTML5 video. Here is a <a href="rabbit320.mp4">link to the video</a> instead.</p>
</video>
```
    * if you remove the controls attribute, there are no controls unless you program them in yourself

* as an aside, this article has really great instructions on how to program and style your own video controls. And it's complicated