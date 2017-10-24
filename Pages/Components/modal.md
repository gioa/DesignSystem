# Modal

**When to use:**

* Need input from the user without losing the context of the page
* Inform user about a task and require decisions 
* Use sparingly as they are interruptive  

**Interaction**

* No other interactions on the main page can be accessed. 
* Dismiss and main action. 
* Scrolling: pinned title and actions on the screen

**Styles**

```css
Title: {
    fontSize: typeSizes[7],            // 13px
    lineHeight: typeLineHeight[7],     // 18px
    fontFamily: fontFamilies.body,     // Helvetica Neue
    fontWeight: fontWeights.regular,   // 400
}

Dialog: {
    width: 
    height:
    padding: 
}

Button: {
    width:
    height:
}
```

**Example**

* Confirmation dialog 
* Simple dialog like create a notebook. 
* Alerts



