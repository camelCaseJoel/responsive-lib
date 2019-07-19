Responsive lib
==============

A 12 columns grid based CSS Responsive library. Something like bootstrap(in spirit) but much simpler. Wrote this little library for a Responsive design tutorial I'm planning to write.

How they work:
--------------

* Use class **.responsive-container** for any HTML element that has a column class
* Column classes are based in a 12 column "grid".
* **small, mid, large** are the different screen sizes.
* Use these column classes like you would use Bootstrap clases:
```
<div class="responsive-container" id="example-1">
	<div class="w-2-of-12-large w-4-of-12-mid w-12-of-12-small">
		Lorem, ipsum dolor sit amet consectetur adipisicing elit.</div>
	<div class="w-2-of-12-large w-4-of-12-mid w-12-of-12-small">
		Lorem, ipsum dolor sit amet consectetur adipisicing elit.</div>
	<div class="w-2-of-12-large w-4-of-12-mid w-12-of-12-small">
		Lorem, ipsum dolor sit amet consectetur adipisicing elit.</div>
	<div class="w-2-of-12-large w-4-of-12-mid w-12-of-12-small">
		Lorem, ipsum dolor sit amet consectetur adipisicing elit.</div>
	<div class="w-2-of-12-large w-4-of-12-mid w-12-of-12-small">
		Lorem, ipsum dolor sit amet consectetur adipisicing elit.</div>
	<div class="w-2-of-12-large w-4-of-12-mid w-12-of-12-small">
		Lorem, ipsum dolor sit amet consectetur adipisicing elit.</div>
</div>
```
* You can nest as many HTML elements as you want:

```
<div class="responsive-container" id="example-2">
	<div class="w-4-of-12-large w-4-of-12-mid w-12-of-12-small">
		Lorem, ipsum dolor sit amet consectetur adipisicing elit.
	</div>
	<div class="w-4-of-12-large w-4-of-12-mid w-12-of-12-small">
		Lorem, ipsum dolor sit amet consectetur adipisicing elit.
	</div>
	<div class="w-4-of-12-large w-4-of-12-mid w-12-of-12-small">
		Lorem, ipsum dolor sit amet consectetur adipisicing elit.
	</div>
	<div class="w-4-of-12-large w-4-of-12-mid w-12-of-12-small">
		Lorem, ipsum dolor sit amet consectetur adipisicing elit.
	</div>
	<div class="responsive-container w-4-of-12-large w-4-of-12-mid w-12-of-12-small">
			<div class="w-6-of-12-large">Lorem, ipsum dolor sit amet consectetur adipisicing elit.</div>
			<div class="w-6-of-12-large">Lorem, ipsum dolor sit amet consectetur adipisicing elit.</div>
		</div>
	<div class="responsive-container w-4-of-12-large w-4-of-12-mid w-12-of-12-small">
		<div class="w-6-of-12-large">Lorem, ipsum dolor sit amet consectetur adipisicing elit.</div>
		<div class="responsive-container w-6-of-12-large">
			<div class="w-6-of-12-large">Lorem, ipsum dolor sit amet consectetur adipisicing elit.</div>
			<div class="w-6-of-12-large">Lorem, ipsum dolor sit amet consectetur adipisicing elit.</div>
		</div>
	</div>
</div>
``` 

These are all the classes:
--------------------------

```
.responsive-container {
    
    overflow: auto;
}
.responsive-container > * {
    float: left; 
}


/* Based in a 12 columns grid */

/* large */
@media ( min-width: 1000px ) {
    .w-1-of-12-large { width: 8.33%; }
    .w-2-of-12-large { width: 16.66%; }
    .w-3-of-12-large { width: 25%; }
    .w-4-of-12-large { width: 33.33%; }
    .w-5-of-12-large { width: 41.66%; }
    .w-6-of-12-large { width: 50%; }
    .w-7-of-12-large { width: 58.33%; }
    .w-8-of-12-large { width: 66.66%; }
    .w-9-of-12-large { width: 75%; }
    .w-10-of-12-large { width: 83.33%; }
    .w-11-of-12-large { width: 91.66%; }
    .w-12-of-12-large { width: 100%; }

}
/* mid */
@media ( max-width: 999px ) {
    .w-1-of-12-mid { width: 8.33%; }
    .w-2-of-12-mid { width: 16.66%; }
    .w-3-of-12-mid { width: 25%; }
    .w-4-of-12-mid { width: 33.33%; }
    .w-5-of-12-mid { width: 41.66%; }
    .w-6-of-12-mid { width: 50%; }
    .w-7-of-12-mid { width: 58.33%; }
    .w-8-of-12-mid { width: 66.66%; }
    .w-9-of-12-mid { width: 75%; }
    .w-10-of-12-mid { width: 83.33%; }
    .w-11-of-12-mid { width: 91.66%; }
    .w-12-of-12-mid { width: 100%; }
}
/* small */
@media ( max-width: 600px ) {
    .w-1-of-12-small { width: 8.33%; }
    .w-2-of-12-small { width: 16.66%; }
    .w-3-of-12-small { width: 25%; }
    .w-4-of-12-small { width: 33.33%; }
    .w-5-of-12-small { width: 41.66%; }
    .w-6-of-12-small { width: 50%; }
    .w-7-of-12-small { width: 58.33%; }
    .w-8-of-12-small { width: 66.66%; }
    .w-9-of-12-small { width: 75%; }
    .w-10-of-12-small { width: 83.33%; }
    .w-11-of-12-small { width: 91.66%; }
    .w-12-of-12-small { width: 100%; }
}
```
