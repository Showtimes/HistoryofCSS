### First Tube CSS Browser Presentation 

Inspired by a few web presentation tools 

### How to make a slide

Copy This section of HTML and duplicate it under the pervious one.
Put everything you need inside the content.

````
<section id="slide-1" class="slide-holder">
	<div class="main-slide slide">
    <div class="front-slide">
      <div class="content">
		    <p>Some information goes here!</p>
      </div>
      <div class="arrow-container right">
        <label for="slide-2-ck" class="arrow arrow-right"></label>
      </div>
    </div>
	</div>
</section>
`````

Arrow container is to wrap the navigation arrow, you can add another one and put 'left' class in order to make arrow container for previous navigation. Don't forget to fill up the attribute 'for' with desired page input id.
````
<div class="arrow-container left">
  <label for="slide-1-ck" class="arrow arrow-left"></label>
</div>
`````


Add your presentation control

```
<input id="slide-3-ck" class="slide-3-ck main-slide slide-input" name="slide" type="radio" />
````

Copy and paste this line of CSS into the area called "Presentation Flow". Increments of 100% work good put experiment with right, left, up down.

````
input.slide-1-ck:checked ~ #slide-container{
    left: 0;
}
````

### To Do
 1. Add in more transition (Done)
 2. Create back button to go to pervious slides (Done)
 3. Add presentation end of time bar 
 4. Add title element

#### Credits and Inspiration

Inspiration: http://www.inwebson.com/css3/pure-css-slideshow-effect-for-presentation/
Arrows: http://codepen.io/eMaj/pen/joLqt
space ship: http://codepen.io/alexsafayan/pen/Bwgnk
http://codepen.io/rpdasilva/pen/sovAB
