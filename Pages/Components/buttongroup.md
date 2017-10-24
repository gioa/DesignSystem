# Button Group

| Class | Example |
| -- | -- | 
| button group |<div class="db"><div class="btn-group"><button class="btn">All</button><button class="btn">Created by me</button><button class="btn selected">Accessible by me</button></div>|

//todo: add javascript to select another option

**When to use**

* Use a button group as a way to select an option
* Select less than 6 options \(Use **Form/Select** for equal or greater than 6 options\)

**Interaction**

* Works as a tab but the style is different
* hover, selected, disabled

**Style**

```less
.btn-group {
    
    button.btn {
      .text-basic;
      border: 1px solid @border-medium;
      background-color: @white;
      border-right-width: 0px;
      outline: none;

      &.selected {
        border-color: @border-blue;
        background-color: @item-active-bg;

        & + button.btn {
          border-left-color: @border-blue;
        }
      }

      &:hover {
        background-color: @item-hover-bg;
      }

      &:first-child {
        border-radius: @border-radius-base 0px 0px @border-radius-base;
      
      }

      &:last-child {
        border-right-width: 1px;
        border-radius: 0px @border-radius-base @border-radius-base 0px;
      
      }

      & + button.btn {
        margin-left: 0;
      }
    }
}
```

**Examples**

* Filter on cluster list page \(All, created by me, accessible by me\)
* Job - add library \(Workspace, DBFS/S3\)
* Create cluster \(Severless and Standard\)



