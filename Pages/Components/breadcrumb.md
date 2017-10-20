# Breadcrumb

Display on the top left corner of the screen, above the page title, subject to top navigation

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

```css
Text style: {
    fontSize: typeSizes[7],            // 13px
    lineHeight: typeLineHeight[7],     // 18px
    fontFamily: fontFamilies.body,     // Helvetica Neue
    fontWeight: fontWeights.regular,   // 400
}

Clickable:{
    color: colors.@black-alpha-500,      //to replace
}
ClickableHover:{
    color:  @black-alpha-800,
}
Nonclickable:{
    color: @black-alpha-300,
}
```

**Example**

* Clusters/Shared Autoscaling



