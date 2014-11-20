jQueryAnimatedChart
===================

Animated jQuery pie chart built on top of [jQuery Knob](http://anthonyterrien.com/knob/). Chart has a colored circle label that has a title, a tagline and a percentage value. Chart can be customized through SCSS.

## Example
``` html
<div id="chart" class="chart_wrapper">
    <input type="text" class="dial chart_anim_1" data-fgColor="#fff" data-bgColor="#ccc"  />
    <div class="circle gray light">
        <span class="title">Chart Title 1</span>
        <span class="tagline">tagline</span>
        <span class="pie_value" id="eh_value">%</span>
    </div>
</div>
```