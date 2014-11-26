jQueryAnimatedChart
===================

Animated jQuery pie chart built on top of [jQuery Knob](http://anthonyterrien.com/knob/). Chart has a colored circle label that has a title, a tagline and a percentage value. Chart can be customized through [SCSS](http://sass-lang.com/). 

## Requirements
* jQuery (tested with v1.11.1)
* [jQuery Knob](http://anthonyterrien.com/knob/)

## Documentation
Be sure to include the `css/main.css` and `js/jquery.knob.js`. The HTML below is using the circle label. If you do not wish to use the circle label, you may exclude the `div` with the `circle` class. 

``` html
<div class="chart_wrapper">
    <input id="chart_anim_1"type="text" class="dial" data-fgColor="#fff" data-bgColor="#ccc"  />

    <!-- gray circle label -->
    <div class="circle gray light">
        <span class="title">Chart Title 1</span>
        <span class="tagline">tagline</span>
        <span class="pie_value" id="eh_value">%</span>
    </div>
</div>
```

If you do not use the label, you need to include `data-width` and `data-height` on your `input` element. Also, in this case, the `chart_wrapper div` is optional.

``` html
<div class="chart_wrapper">
    <!-- no circle label -->
    <input id="chart_anim_3"type="text" class="dial" data-fgColor="#444444" data-bgColor="#ccc" data-width="225" data-height="225" />
</div>
```
### Start the animation
Call `animateChart` to set the initial and final value, and to trigger animation.

``` javascript
animateChart('chart_anim_1', 0, 79); // Animates chart with ID 'chart_anim_1' from 0 to 79
```

### Customize SCSS
* __$pie_chart_dia__: pie chart diameter
* __$circle_label_dia__: circle label diameter

## Compatibility
Tested on [Firefox](https://www.mozilla.org/en-US/firefox/new/) 33.1, [Chrome](http://www.google.com/chrome/) 38.0, [Safari](https://www.apple.com/safari/) 8.0, Mobile Safari 7.0, [Android Chrome](https://play.google.com/store/apps/details?id=com.android.chrome&hl=en) 39.0.

## License
jQueryAnimatedChart is licensed under the [MIT License](http://opensource.org/licenses/MIT).