# Timing of value changes #

[Demo](https://MERNCraft.github.io/timing)

This CSS-only page illustrates the timing of changes to `z-index` during an animation.

Properties like `z-index`, `grid`, `content` and `counter`s take discrete properties. During an animation these will switch abruptly from one discrete value to another. When this happens depends on the [`animation-timing-property`](https://developer.mozilla.org/en-US/docs/Web/CSS/animation-timing-function#stepsn_jumpterm) interpolation method. For values which represent progressive interpolations, like `linear`, the discrete properties switch value half-way between keyframes.

This is described in more detail [here](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_animated_properties).

Other animatable properties, like `color`, `left` and `opacity`, can have values which vary smoothly over time. These can be made to proceed step-wise by using a `step-` or `jump-` value for the `animation-timing-property`.

This demo allows you to compare these behaviours.

You can find a list of all animatable CSS properties [here](https://www.quackit.com/css/css3/animations/animatable_properties/). Most properties have an animation associated with them, and code that you can copy and paste.
