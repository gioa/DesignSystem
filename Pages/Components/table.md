# Table

**When to use**

* Use tables to logically structure content in a grid to facilitate understanding

**Interaction**

* Row hover, select, disabled 
* Truncation in long text: display full text in tooltip on hover 
* Sorting on column
* Filtering
* Scrolling  
* Pagination 
* Links and actions 
* Empty values

**Styles**

```css
header: {
    background-color: ,
    color:,
    fontSize: typeSizes[7],            // 13px
    lineHeight: typeLineHeight[7],     // 18px
    fontFamily: fontFamilies.body,     // Helvetica Neue
    fontWeight: fontWeights.regular,   // 400

    width:
    height:

    sort column{
        arrow icon 
    }
    sort column{
        indicate column is sortable
    }
}

row:{
    width 
    height 

}
row:hover{
    background-color:
}
row:disable{
    background-color:
}

cell{
    cell width:
    padding:
}




column alignment:{
    left align text columns
    right align numeric column
}
```

**Example**

* Cluster list page, job list page, IAM role table, user table 
* sample data table and schema table in table detail page



