# Spacing

Use **multiples of 4 **to define dimension, padding and margin of both block and inline elements. Learn more about [8-pt grid](https://spec.fm/specifics/8-pt-grid).

**When to use **

* Define padding, margin of both block and inline elements
* Define dimension \(width and height\)

##### Spacing

```js
const spacing = {
    zero: 0,
    small: 4,
    base: 8,
    medium: 12,
    large: 16,
    x-large:24,
    xx-large: 32,
    xxx-lage: 48,
}
```

##### Element dimensions

```js
// todo: consolidate the values. 
// Too specific at the foundation level? Defined in component level instead?

const width =  {
    sidebar: 76,  
    filetree: 196,
    right-panel: 250,
    tooltip:260,
    form: 300;
    dialog-small: 400,
    dialog-medium:600,
    dialog-big:800,
    find-and-replace-bar: 1000,
}

const height = {
    button: 28,
    topbar: 40,
    dropdown-max: 600,//?
    dialog-max: 600,

};
```



