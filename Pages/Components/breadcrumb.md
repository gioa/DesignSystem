# Breadcrumb

Display on the top left corner of the screen, above the page title, subject to top navigation.

| Class | Example |
| -- | -- | 
| breadcrumb |<div class="db"><div class="breadcrumb"><a>Clusters</a>/Create cluster</div>|



**When to use**

* Help user visualize current location by showing the hierarchy of pages \(e.g., notebook path in workspace\)
* Use when the user is most likely to have landed from an external source \(e.g., job run result page\)
* Use across the product to maintain consistency 

**Interaction**

* Use button link to link to that section or page
* When exceed the content width, use \(...\) between the entities.
* Clicking on \(...\) will expand, if no spacing, overflow or scrollable?
* Super long entity name are truncated and use a tooltip to show the full name

**Styles**

```less
.breadcrumb{	
	.text-basic;
	
	a{
		color: @link-gray;
		
		&:hover{
			color: @text-basic-color;
			text-decoration: none;
		}
	}
}
```

**Example**

* Clusters/Shared Autoscaling



