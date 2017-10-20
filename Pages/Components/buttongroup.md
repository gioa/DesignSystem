# Button Group

Use a button group as a way to select an option.

**When to use**

* Select less than 6 options \(Use **Form/Select** for equal or greater than 6 options\)

**Interaction**

* Works as a tab but the style is different
* hover, selected, disabled

**Styles for different states**

```css
TextStyle: {
    fontSize: typeSizes[7],            // 13px
    lineHeight: typeLineHeight[7],     // 18px
    fontFamily: fontFamilies.body,     // Helvetica Neue
    fontWeight: fontWeights.regular,   // 400
}

Regular{
    border: solid 1px colors.gray300,  // #ccc
    background-color: colors.white, 
    padding: spacing[0] spacing[3],    // 4px, 16px  
}

hover{
    border: solid 1px colors.gray300,  
    background-color: colors.gray100, // #f5f5f5
}

selected{
    border: solid 1px colors.blue600, 
    background-color: colors.gray200, // #eee 
}

disable{
    opacity: disabledOpacity,         // 0.45
}
```

**Styles for different positions**

```css
leftmost{
    border-radius: radius[1] 0,      //4
}
middle{
    border-radius: 0,
}
rightmost{
    border-radius: 0 radius[1] ,     //4
}
```

**Examples**

* Filter on cluster list page \(All, created by me, accessible by me\)
* Job - add library \(Workspace, DBFS/S3\)
* Create cluster \(Severless and Standard\)



