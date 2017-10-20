# Tooltip

**When to use:**

* When hover over a UI element \(truncated text, icon\), a tooltip appears to provide additional information. 
* Sometimes behavior as coach marks to guide user take certain actions \(e.g., create a new cluster, enter dashboard name\).   

**Interaction**

* Allow hover and copy the text 
* Dismiss when move away 

**Styles**

```css
text: {
    fontSize: typeSizes[7],            // 13px
    lineHeight: typeLineHeight[7],     // 18px
    fontFamily: fontFamilies.body,     // Helvetica Neue
    fontWeight: fontWeights.regular,   // 400
}

box: {
    color: colors.white,               // todo
    background-color: colors.gray100,
    border-radius:, 
    width: ,
}
```

**Example**

* Tooltip icon near the input field label
* Tooltip for cluster actions on cluster list page



