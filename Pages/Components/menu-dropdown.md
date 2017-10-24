# Menu Dropdown

Display a list of options with one option per line.

| Class | Example |
| -- | -- | 
| dropdown |<div class="db"><div class="dropdown-menu"><ul><li><a href="#">Action</a></li><li><a href="#">Another action</a></li><li><a href="#" disabled>Disabled action</a></li><li><a href="#">Something else here</a></li><li role="separator" class="divider"></li><li><a href="#">Separated link</a></li></ul></div>|

**When to use**

* Offer users a list of actions \(e.g., user menu\) or options to select \(dropdown in form/select element\)
* Contain at least 2 items

**Interaction**

* Appear when click on an icon, e.g., File menu, or user menu on the top right
* Appear close to the UI element where it get activated, above all other UI elements.  
* Dismiss by clicking elsewhere or select a menu item. 
* Disable state
* Scrollable 
* Cascading menu 
* Menu nesting: reveal nested submenus, nested to one level deep only.  

**Style**

```less
.dropdown-menu {
    display: block;
    position: relative;
    z-index: @zindex-dropdown;
    min-width: @width-dropdown-min;
    max-width: @width-dropdown-max;
    
    background: @white;  
    border-radius: @border-radius-base;
    border: 1px solid @border-medium;
    box-shadow: @box-shadow;
    padding: 0px;
    
    > ul {
        overflow: auto;
        list-style: none;
        margin: 0px;      
        padding: @spacing-small 0;

        > li {
            margin: 0px;
            padding: 0px;
            position: relative;

            &.divider {
                height: 1px;
                margin: @spacing-small 1px;
                background-color: @border-light;
            }

            &.dropdown-header {
                padding: @spacing-small @spacing-base;
                .text-small;
                color: @text-secondary-color;
            }

            > a {
                padding: @spacing-small @spacing-base;
                cursor: default;
                color: inherit;
                text-decoration: none;
                display: block;
                .text-overflow;
                cursor: pointer;
                text-shadow: none;

                &:not([DISABLED]):hover {
                    text-decoration: none;
                    text-shadow: none;
                    background: @blue-green-100;
                    color: @white;

                }
                &.disabled, &[disabled], &.disabled:hover {
			        opacity: @disabled-opacity-base;
			    }
            }
        }
    }
}
```

**Example**

* User menu 
* Notebook menu dropdown 
* Notebook cell actions 



