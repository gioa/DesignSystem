# Spacing

Use **multiples of 4 **to define dimension, padding and margin of both block and inline elements. Learn more about [8-pt grid](https://spec.fm/specifics/8-pt-grid).

**When to use **

* Define padding, margin of both block and inline elements
* Define dimension \(width and height\)

##### Spacing

```less
@spacing-zero: 0px;
@spacing-small: 4px;
@spacing-base: 8px;
@spacing-medium: 12px;
@spacing-large: 16px;
@spacing-x-large: 24px;
@spacing-xx-large: 32px;
@spacing-xxx-large: 48px;
```

##### Element dimensions

```less
// todo: consolidate the values. 
// Too specific at the foundation level? Defined in component level instead?

// width 
@width-sidebar: 76px;
@width-filetree: 196px;
@width-rightpanel: 250px;
@width-tooltip: 260px;
@width-form-login: 300px;
@width-dialog-small: 400px;
@width-dialog-base: 600px;
@width-dialog-large: 800px;

// height 
@height-button: 28px;
@height-topbar: 40px;
@height-component-max: 600px;
```



