# Button


| Class | Example |
| -- | -- | 
| btn |<div class="db"><button type="button" class="btn  btn-default">Default</button> <button type="button" class="btn  btn-default" disabled>Default</button> <button type="button" class="btn btn-default"><i class="fa fa-close"></i></span> Terminate </button> </div>|
| btn btn-primary |<div class="db"><button type="button" class="btn  btn-primary">Primary</button> <button type="button" class="btn  btn-primary" disabled>Primary</button>  <button type="button" class="btn btn-primary"><i class="fa fa-plus"></i></span> Create Cluster</button></div>|
| btn  btn-danger |<div class="db"><button type="button" class="btn  btn-danger">Danger</button> <button type="button" class="btn  btn-danger" disabled>Danger</button></div>|
| btn btn-fit-container |<div class="db"><button type="button" class="btn  btn-primary btn-fit-container">Sign In</button></div>|

### Default

**When to use**

* Use button to trigger an action
* Along with primary button \(e.g., cancel\)
* Multiple actions \(clone, restart, terminate on cluster detail page\)

##### Style

```less
.btn {
    .text-basic;
    border-radius: @border-radius-base;
    padding: @spacing-small @spacing-base;
    background: @item-active-bg;
    border: 1px solid @border-medium;
    text-decoration: none;
    text-shadow: none;
    cursor: pointer;
    display: inline-block;
    
    /* States */
    &:not([DISABLED]):hover, &:not([DISABLED]):active, &:not([DISABLED]):focus{
        background: @item-hover-bg;
    }

    &:focus, &:active, &:hover {
        outline: none;
    }

    &.disabled, &[disabled], &.disabled:hover {
        cursor: not-allowed;
        opacity: @disabled-opacity-base;
    }
}
```

_Usage_: Cancel, Cluster actions, e.g., Clone, Restart, Terminate

### Primary

**When to use**

* To call out an action on a form or a page. E.g., Create. Confirm. Save.
* Add icon to draw more attention and give more context visually. E.g, + New cluster
* Icon only when space is constrained and the icon is obvious for the action. 

**Interaction**

* Add hover state to give users feedback. 
* Disable button when action is unavailable. Show why and inform users how to enable it.
* When an action takes a while, show loading states.  
* For icon only button, add label in the tooltip.

##### Styles

```less
.btn-primary{
    background: @blue-green-100;
    color:@white;
    border: 1px solid @blue-green-100;

    &:not([DISABLED]):hover, &:not([DISABLED]):active, &:not([DISABLED]):focus {
        background: @blue-green-200;
    } 
}

```

_Usage_: Create cluster, create job, Save, Confirm

### Danger

**When to use**

* Destructive actions such as delete or remove to call attention.

##### Style

```less
.btn-danger{
    background: @red-500;
    color: @white;
    border: 1px solid @red-700;

    &:not([DISABLED]):hover, &:not([DISABLED]):active, &:not([DISABLED]):focus {
        background: @red-700;
    } 
}
```

_Usage_: Remove User, Disable ACLs, Delete dashboard (fit container)


### Fit container

**When to use**

* Emphasize the key action per container

##### Style

```less
.btn-fit-container{
    .text-large;
    display:block;
    text-align: center;
    width: 100%;
    padding-top: @spacing-base;
    padding-bottom: @spacing-base;
}
```

_Usage_: Sign In, Single Sign On, Back to sign in button in choose organization page


### Icon

**When to use**

* Icon only when space is constrained and the icon is obvious for the action. 

**Styles**

```
// todo
```

_Usage_: add cell and paste cell, comments, notebook plot options 



