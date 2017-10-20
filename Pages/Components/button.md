# Button

Use a button to trigger an action. Button style varies based on their types/sizes/states.

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

##### Primary: regular

```css
PrimaryButton: {
    background-color: colors.blue500,  // todo: replace with bluegreen100?
    color: colors.white,               // #fff
    border: solid 1px colors.blue600,  // border style
    border-radius: radius[1],          // 4px
    padding: spacing[0] spacing[1],    // 4px, 8px  
    fontSize: typeSizes[7],            // 13px
    lineHeight: typeLineHeight[7],     // 18px
    fontFamily: fontFamilies.body,     // Helvetica Neue
    fontWeight: fontWeights.regular,   // 400
}
```

**Styles for different states**

```css
PrimaryButtonHover:{
    background-color: colors.blue700,  
}

PrimaryButtonDisable:{
    opacity: disabledOpacity,          // 0.45
}

PrimaryButtonLoading:{
    opacity: disabledOpacity,          // 0.45
    fa-spinner: display,               // to do  
}
```

**Primary: icon + label **

```css
PrimaryButtonIcon: {
    i.fa-xxx{
        margin-right: spacing[0],      //4px 
    }
}
```

_Usage:_ Create button on cluster list page

**Primary: fit container + bigger **

```css
PrimaryButtonFitContainer: {
    background-color: colors.blue500, // todo: replace with bluegreen100?
    color: colors.white,              // #fff
    border: solid 1px colors.blue600, // border style
    border-radius: radius[1],          // 4px
    padding: spacing[1] auto,         // 8px, auto 
    fontSize: typeSizes[6],           // 14px
    lineHeight: typeLineHeight[6],    // 24px
    fontFamily: fontFamilies.body,    // Helvetica Neue
    fontWeight: fontWeights.regular,  // 400
}
```

_Usage_: Sign In, Single Sign On

### Default

**When to use**

* Along with primary button \(e.g., cancel\)
* Multiple actions \(clone, restart, terminate on cluster detail page\)

##### Default: regular

```css
DefaultButton: {
    background-color: colors.gray.100, // #f5f5f5
    color: colors.gray800,             // #333    
    border: solid 1px colors.gray300,  // border style
    border-radius: radius[1],          // 4px
    padding: spacing[0] spacing[1],    // 4px, 8px
    fontSize: typeSizes[7],            // 13px
    lineHeight: typeLineHeight[7],     // 18px
    fontFamily: fontFamilies.body,     // Helvetica Neue
    fontWeight: fontWeights.regular,   // 400
}
```

_Usage_: Cancel.

**Default: different states **

```css
DefaultButtonHover:{
    background-color: colors.gray200,  // #eee 
}
```

_Usage_: Cancel

**Default: icon + label **

```css
DefaultButtonIcon: {
    i.fa-xxx{
        margin-right: spacing[0],      //4px 
    }
}
```

_Usage_: Cluster actions, e.g., Clone, Restart, Terminate

**Default: fit container + bigger**

```css
FitContainerButtonDefault: {
    background-color: colors.gray.100,  // #f5f5f5
    color: colors.gray800,              // #333
    border: solid 1px colors.gray300,   // border style
    border-radius: radius[1],          // 4px
    padding: spacing[1] auto,           // 8px, auto 
    radius: radius[1], // 4px
    fontSize: typeSizes[6],             // 14px
    lineHeight: typeLineHeight[6],      // 24px
    fontFamily: fontFamilies.body,      // Helvetica Neue
    fontWeight: fontWeights.regular,    // 400
}
```

_Usage_: Back to sign in button in choose organization page

**Default: fit container + icon**

```css
FitContainerButtonDefault: {
    background-color: colors.gray.100, // #f5f5f5
    color: colors.gray800,             // #333
    border: solid 1px colors.gray300,  // border style 
    border-radius: radius[1],          // 4px
    padding: spacing[0] auto,          // 4px, auto 
    radius: radius[1], // 4px
    fontSize: typeSizes[7],            // 13px
    lineHeight: typeLineHeight[7],     // 18px
    fontFamily: fontFamilies.body,     // Helvetica Neue
    fontWeight: fontWeights.regular,   // 400

    i.fa-xxx{
        margin-right: spacing[0], //4px 
    }
}
```

_Usage_: Back to sign in button in choose organization page

### 

### Danger

**When to use**

* Destructive actions such as delete or remove to call attention.

##### Danger: regular

```css
DangerButton: {
    background-color: colors.red500,  
    color: colors.white,               // #fff
    border: solid 1px colors.red700,  // border style
    border-radius: radius[1],          // 4px
    padding: spacing[0] spacing[1]     // 4px, 8px   
    fontSize: typeSizes[7],            // 13px
    lineHeight: typeLineHeight[7],     // 18px
    fontFamily: fontFamilies.body,     // Helvetica Neue
    fontWeight: fontWeights.regular,   // 400
}
```

_Usage_: Remove User, Disable ACLs.

**Danger: different states **

```css
DangerButtonHover:{
    background-color: colors.red700,  
}

DangerButtonDisable:{
    opacity: disabledOpacity,          // 0.45
}
```

_Usage_: Remove user, Disable ACLs.

**Danger: Icon + Label**

```css
DangerButtonIcon: {
    i.fa-xxx{
        margin-right: spacing[0],      //4px 
    }
}
```

_Usage_: Delete dashboard

**Danger: Fit container + Icon**

```css
DangerButtonFitContainerIcon: {
    background-color: colors.red500,  
    color: colors.white,              // #fff
    border: solid 1px colors.red700,  // border style
    border-radius: radius[1],          // 4px
    padding: spacing[0] auto, // 4px, auto
    fontSize: typeSizes[7], // 13px
    lineHeight: typeLineHeight[7], // 18px
    fontFamily: fontFamilies.body, // Helvetica Neue
    fontWeight: fontWeights.regular, // 400

    i.fa-xxx{
        margin-right: spacing[0], //4px
    }
}
```

_Usage_: Delete dashboard

### Icon

**When to use**

* Icon only when space is constrained and the icon is obvious for the action. 

**Styles**

```
// todo
```

**Example**

* add cell and paste cell
* comments
* actions in a table \(flat icon\)
* notebook plot options 



