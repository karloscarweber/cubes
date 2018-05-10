# Colors

Cheddar uses simple presets for whites and blacks, with a few brand tones for special elements.

### Greyscale Colors

<div class="grater">
  <div class="bg-white-one f3">
    <p class="black-one">.black-one</p>
    <p class="black-two">.black-two</p>
    <p class="black-three">.black-three</p>
    <p class="black-four">.black-four</p>
  </div>
  <div class="bg-black-one f3">
    <p class="bg-white-one">.white-one</p>
    <p class="bg-white-two">.white-two</p>
    <p class="bg-white-three">.white-three</p>
    <p class="bg-white-four">.white-four</p>
  </div>
</div>

### Application Colors

<div class="grater">
  <div class="bg-white-one f3">
    <p class="cheddar-orange">.cheddar-orange</p>
    <p class="cheddar-blue">.cheddar-blue</p>
    <p class="cheddar-yellow">.cheddar-yellow</p>
  </div>
  <div class="bg-black-one f3">
    <p class="white-one bg-cheddar-orange">.bg-cheddar-orange</p>
    <p class="white-one bg-cheddar-blue">.bg-cheddar-blue</p>
    <p class="black-one bg-cheddar-yellow">.bg-cheddar-yellow</p>
  </div>
</div>

<pre>
/*

   Cubes
   COLORS

*/

:root {
  --black-one: #383838;
  --black-two: #494949;
  --black-three: #969696;
  --black-four: #b9b9b9;

  --white-one: #ffffff;
  --white-two: #f9f9f9;
  --white-three: #f3f3f3;
  --white-four: #e4e4e4;

  --cheddar-orange: #ff723a;
  --cheddar-blue: #198eff;
  --cheddar-yellow: #ffe33a;
}

</pre>

### Skinning Convenience Classes

As a convenience all colors can be used to style any elements `color` or `background-color`. the convenience classes are the ones used above in the examples.

<pre>
/*

   Cubes
   Text Colors & Backgrounds

   Skins

*/

/* Text colors */

.black-one {
  color: var(--black-one);
}
.black-two {
  color: var(--black-two);
}
.black-three {
  color: var(--black-three);
}
.black-four {
  color: var(--black-four);
}

.white-one {
  color: var(--white-one);
}
.white-two {
  color: var(--white-two);
}
.white-three {
  color: var(--white-three);
}
.white-four {
  color: var(--white-four);
}

.cheddar-orange {
  color: var(--cheddar-orange);
}
.cheddar-blue {
  color: var(--cheddar-blue);
}
.cheddar-yellow {
  color: var(--cheddar-yellow);
}

/* Background */

.bg-black-one {
  background-color: var(--black-one);
}
.bg-black-two {
  background-color: var(--black-two);
}
.bg-black-three {
  background-color: var(--black-three);
}
.bg-black-four {
  background-color: var(--black-four);
}

.bg-white-one {
  background-color: var(--white-one);
}
.bg-white-two {
  background-color: var(--white-two);
}
.bg-white-three {
  background-color: var(--white-three);
}
.bg-white-four {
  background-color: var(--white-four);
}

/* Background colors */

.bg-cheddar-orange {
  background-color: var(--cheddar-orange);
}
.bg-cheddar-blue {
  background-color: var(--cheddar-blue);
}
.bg-cheddar-yellow {
  background-color: var(--cheddar-yellow);
}
</pre>
