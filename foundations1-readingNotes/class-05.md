# HTML & CSS

## Chapter 5: Images (p.94-125)

* Good practice to have all of your images in one folder
* To add images use ```<img/>```
    * must include ```src``` (the location of where to get the image) and ```alt``` (a description of the image for screen readers)
* Can specify the height and width of the image in HTML which helps with the speed of the page loading
* Where you place the image in your code effects where it shows up on the page
* ```align``` is used to tell the rest of the text how to flow around the image
    * ```align=left``` would mean the image is aligned to the left side of the page, allowing text to flow around the right hand side
* images should be saved in the correst format, at the right size and measured in pixels
    * jpeg should be used for photos and images with many colors, gif or png can be used for images with few or large areas of the same color
* ```<figure>``` can be used to wrap an image with it's ```<figcaption>```

## Chapter 11: Color (p.246-263)

* *foreground color* refers to the color of text inside of an element and uses ```color: grey```
* *background color* refers to the color of the backfround and uses ```background color: purple```
* *opacity* can be changed as the 4th property of an RGB color

## Chapter 12: Text (p.264-299)

* can specify font using ```font-family: name of font```
* change font size with ```font-size:``` in pixels, percentages or ems (which is equivalent to the width of a letter m!)
* ```font-weight``` can be bold or normal
* ```font-style``` can be italic, normal or oblique
* ```text-transform``` can be all uppercase, all lowercase or capitalize (which causes the 1st letter of each word to be capitalized)
* with ```text-decoration``` you can add underline, overline, line-through or blink(which makes the text blink on and off)
* can change the leading with ```line-height``` and letter and word spacing with ```letter-spacing``` and ```word-spacing``` (adjusts kerning)
* align text horizontially with ```text-align: left, right, center or justify```
* align text vertically with ```vertical-align: baseline, sub, super, top, text-top, middle, bottom, text-bottom```
* ```text-indent``` indents the first line of text
* ```text-shadow``` creates a drop shadow behind your word
    * takes three values and a color for the shadow (use a generator)
* can style first letter or first line differently with ```first-letter: or first-line:```
* can change the color of links provided with ```link: {color:blue} or visited:{color: pink}```