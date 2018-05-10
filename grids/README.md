# Grids

Cheddar uses [Grater](https://github.com/karloscarweber/grater) from the original Cheddar to create a grid. All elements are either narrow or not. It's a simple 2 column system that assumes that you want everything to be 1 column on mobile.

![Grater example expanded](/grater-example1.png)
![Grater example narrow](/grater-example2.png)

## Usage

add the `.grater` class to a containing div, child divs are assumed to be kept to 2 and are then split between both of these sections.

An example:

<pre>
&lt;div class="grater"&gt;
  &lt;div&gt;
    &lt;p&gt;This is on the left or on top when things get narrow.&lt;/p&gt;
  &lt;/div&gt;
  &lt;div&gt;
    &lt;p&gt;This is on the right or on the bottom when things get narrow.&lt;/p&gt;
  &lt;/div&gt;
&lt;/div&gt;
</pre>

<div class="grater">
  <div class="bg-white-three">
    <p>This is on the left or on top when things get narrow.</p>
  </div>
  <div class="bg-white-three">
    <p>This is on the right or on the bottom when things get narrow.</p>
  </div>
</div>

<pre>
/*

   Grater
   Super Simple Grids

   https://github.com/karloscarweber/grater

*/

.grater-container {
  width: 640px;
  margin: 0 auto;
}
@media all and (max-width: 660px) {
  .grater-container {
    width: 300px;
  }
}
.grater {
  zoom: 1;
}
.grater > div {
  width: 300px;
  margin: 0 0 2em;
}
.grater > div:first-child {
  float: left;
}
.grater > div:last-child {
  float: right;
}
.grater.reverse > div:first-child {
  float: right;
}
.grater.reverse > div:last-child {
  float: left;
}
.grater:before,
.grater:after {
  content: "";
  display: table;
}
.grater:after {
  clear: both;
}
@media all and (max-width: 660px) {
  .grater {
    margin-bottom: 1em;
  }
  .grater > div {
    float: none !important;
    margin: 0 auto 2em;
  }
}

</pre>
