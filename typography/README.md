# Typography

The typeface, it's size, rhythm, and leading have almost everything to do with the feel and personality of a website or application. It's the first brand ambassador.

## Font Size

Font size is set using `rem` as a unit. `rem` uses the font size set for the entire html document as the base for all type sizes. The expected core font size is `16px`, and the core line height is `24px`. We use a pixel size as a base and `rem`s to set the actual font size of text elements to allow users to adjust their font size without breaking the rhythm we've established.

<ul class="list">
  <li><span class="f-headline lh-solid b">C</span><br><span class="f5">6rem (96px)</span></li>
  <li><span class="f-subheadline lh-solid b">C</span><br><span class="f5">5rem (80px)</span></li>
  <li><span class="f1 lh-copy b">C</span><br><span class="f5">3rem (48px)</span></li>
  <li><span class="f2 lh-copy b">C</span><br><span class="f5">2.25rem (36px)</span></li>
  <li><span class="f3 lh-copy b">C</span><br><span class="f5">1.5rem (24px)</span></li>
  <li><span class="f4 lh-copy b">C</span><br><span class="f5">1.25rem (20px)</span></li>
  <li><span class="f5 lh-copy b">C</span><br><span class="f5">1rem (16px)</span></li>
  <li><span class="f6 lh-copy b">C</span><br><span class="f5">.875rem (14px)</span></li>
</ul>

<pre>
/*

   TYPE SCALE
   Docs: http://tachyons.io/docs/typography/scale/

   Base:
    f = font-size

   Modifiers
     1 = 1st step in size scale
     2 = 2nd step in size scale
     3 = 3rd step in size scale
     4 = 4th step in size scale
     5 = 5th step in size scale
     6 = 6th step in size scale
     7 = 7th step in size scale

   Media Query Extensions:
     -ns = not-small
     -m  = medium
     -l  = large
*/

/*
 * For Hero/Marketing Titles
 *
 * These generally are too large for mobile
 * so be careful using them on smaller screens.
 * */

.f-6,
.f-headline {
  font-size: 6rem;
}
.f-5,
.f-subheadline {
  font-size: 5rem;
}


/* Type Scale */

.f1 { font-size: 3rem; }
.f2 { font-size: 2.25rem; }
.f3 { font-size: 1.5rem; }
.f4 { font-size: 1.25rem; }
.f5 { font-size: 1rem; }
.f6 { font-size: .875rem; }
.f7 { font-size: .75rem; } /* Small and hard to read for many people so use with extreme caution */

@media (--breakpoint-not-small){
  .f-6-ns,
  .f-headline-ns { font-size: 6rem; }
  .f-5-ns,
  .f-subheadline-ns { font-size: 5rem; }
  .f1-ns { font-size: 3rem; }
  .f2-ns { font-size: 2.25rem; }
  .f3-ns { font-size: 1.5rem; }
  .f4-ns { font-size: 1.25rem; }
  .f5-ns { font-size: 1rem; }
  .f6-ns { font-size: .875rem; }
  .f7-ns { font-size: .75rem; }
}

@media (--breakpoint-medium) {
  .f-6-m,
  .f-headline-m { font-size: 6rem; }
  .f-5-m,
  .f-subheadline-m { font-size: 5rem; }
  .f1-m { font-size: 3rem; }
  .f2-m { font-size: 2.25rem; }
  .f3-m { font-size: 1.5rem; }
  .f4-m { font-size: 1.25rem; }
  .f5-m { font-size: 1rem; }
  .f6-m { font-size: .875rem; }
  .f7-m { font-size: .75rem; }
}

@media (--breakpoint-large) {
  .f-6-l,
  .f-headline-l {
    font-size: 6rem;
  }
  .f-5-l,
  .f-subheadline-l {
    font-size: 5rem;
  }
  .f1-l { font-size: 3rem; }
  .f2-l { font-size: 2.25rem; }
  .f3-l { font-size: 1.5rem; }
  .f4-l { font-size: 1.25rem; }
  .f5-l { font-size: 1rem; }
  .f6-l { font-size: .875rem; }
  .f7-l { font-size: .75rem; }
}
</pre>

## Line Height

**Line height** follows a simple scale, Text is spaced differently based on their size and we are give 3 options that follow typographic norms: `solid`, `title`, `copy`. `.solid` matches the `line-height` to the text's font-size, which is preferred for large text and headlines. `.title` should be used for titles and `.copy` should be used for all copy and text. `.copy` is most legible with small text and large prose.

**No applied Line Height**

<p class="f5">Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet.</p>

**Line height Solid**

<p class="f5 lh-solid">Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet.</p>

<pre>
/*

   LINE HEIGHT / LEADING
   Docs: http://tachyons.io/docs/typography/line-height

   Media Query Extensions:
     -ns = not-small
     -m  = medium
     -l  = large

*/

  .lh-solid { line-height: 1; }
  .lh-title { line-height: 1.25; }
  .lh-copy  { line-height: 1.5; }

@media (--breakpoint-not-small) {
  .lh-solid-ns { line-height: 1; }
  .lh-title-ns { line-height: 1.25; }
  .lh-copy-ns  { line-height: 1.5; }
}

@media (--breakpoint-medium) {
  .lh-solid-m { line-height: 1; }
  .lh-title-m { line-height: 1.25; }
  .lh-copy-m  { line-height: 1.5; }
}

@media (--breakpoint-large) {
  .lh-solid-l { line-height: 1; }
  .lh-title-l { line-height: 1.25; }
  .lh-copy-l  { line-height: 1.5; }
}
</pre>
