# fifi-Slider
Supports IE10+. Pure JavaScript. Non-jQuery-dependent. CSS3 transition.

[Slider Demo 1 on CodePen](http://codepen.io/fionnachan/pen/Qppdgj)
[Slider Demo 2 on CodePen](http://codepen.io/fionnachan/pen/ryYrpP)

#### For the DOM:
```
.slider
  <!-- repeat below for more slides-->
  .slide
    img(src="your-image-here")
    <!-- you can also have more <div/>s or <p/>s here for text--> 
  <!-- repeat above for more slides-->

.dots-wrapper(id="dots-wrapper-4")
```

#### For the script:

<pre>var test_slider = new fifi_slider({
  target: document.querySelector('.slider'),
  dotsWrapper: document.querySelector('.dots-wrapper'),
  autoplay: { // autoplay function not built yet***
    on: false,
    interval: 1000 // in ms
  },
  transition: {
    speed: 300, // in ms
    easing: '' // CSS3 easing as 'linear' in transition: all 0.6s linear;
  },
  swipe: true, // haven't built arrows function yet, please don't turn it off before arrows are built
  autoHeight: true,
  startSlide: 0, // from 0,
  afterChangeSlide: function afterChangeSlide() {} // customized callback after changing the slide
});</pre>
