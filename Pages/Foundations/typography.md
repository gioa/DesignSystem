# Typography

### Basic variables 

##### When to use

* Use the following variables to define the text styles in the UI components.
* If any is missing, add in font.less.

##### Font family

```less
@text-font: "Helvetica Neue", "Helvetica", "Arial", sans-serif;
@code-font: "Source Code Pro", "Menlo", monospace;
@newslab-font: "Newslab", serif;
@icon-font: "FontAwesome";
```

##### Font size and line height

```less
// font size
@font-size-x-large: 52px; // welcome to
@font-size-large: 33px;// workspace access control
@font-size-h1: 26px; // page title, modal title
@font-size-h2: 22px; // sign in to Databricks, choose organization
@font-size-h3: 18px; // section title
@font-size-h4: 16px;
@font-size-h5: 14px; // 
@font-size-h6: 13px; // file tree title, notebook menu, user menu, dialog text.
@font-size-small: 12px; // language, shift+enter to run
@font-size-x-small: 11px; // sidebar text

// line height
@line-height-x-large: 72px;
@line-height-large: 48px;
@line-height-h1: 36px;
@line-height-h2: 32px;
@line-height-h3: 24px;
@line-height-h4: 24px;
@line-height-h5: 20px;
@line-height-h6: 18px;
@line-height-small: 16px;
@line-height-x-small: 16px;

```

##### Font weight

```less
// weight
@font-weight-bolder: 700;
@font-weight-bold: 500;
@font-weight-base: 400;
@font-weight-light: 200;
```

### Different sizes

| Class | Example |
| -- | -- | 
| headline | <div class="headline">Welcome to</div> |
| title-large | <div class="title-large">Workspace Access Control</div> |
| title-dialog | <div class="title-dialog">Dialog Title </div> |
| title-page | <div class="title-page">Page Title</div> |
| title-section | <div class="title-section">Section Title</div> |
| text-tab | <div class="text-tab">Tab Text</div> |
| text-large | <div class="text-large">Large text</div> |
| text-basic | <div class="text-basic">Basic text</div> |
| text-small | <div class="text-small">Small text</div> |
| text-smaller | <div class="text-smaller">Smaller text</div> |



##### Headline

```less
.headline {
    font-size: @font-size-x-large;
    line-height: @line-height-x-large;
    font-family: @newslab-font;
    color: @black-alpha-300;
}
```

_Usage_: Welcome to Databricks

##### Large Title

```less
 .title-large {
    font-size: @font-size-large;
    line-height: @line-height-large;
}
```

_Usage_: Workspace Access Control \(to be deprecated\)

##### Dialog Title

```less
.title-dialog {
    font-size: @font-size-h1;
    line-height: @line-height-h1;
    font-weight: @font-weight-light;
}
```

_Usage_: Dialog title, Create New Cluster\(to be deprecated\)

##### Page Title

```less
.title-page {
    font-size: @font-size-h2;
    line-height: @line-height-h2;
 }
```

_Usage_: Sign In to Databricks, future page titles

##### Section Title

```less
 .title-section {
    font-size: @font-size-h3;
    line-height: @line-height-h3;
 }

```

_Usage_: Sample Data, Interactive Cluster

##### Large Tab Text

```css
LargeTabText: {
    fontSize: typeSizes[5],            // 16px
    lineHeight: typeLineHeight[5],     // 24px
    fontFamily: fontFamilies.body,     // Helvetica Neue
    fontWeight: fontWeights.regular,   // 400
}
```

_Usage_: Single Sign on / Admin Login

##### Large Body Text

```css
LargeBodyText: {
    fontSize: typeSizes[6],            // 14px
    lineHeight: typeLineHeight[6],     // 20px
    fontFamily: fontFamilies.body,     // Helvetica Neue
    fontWeight: fontWeights.regular,   // 400
}
```

_Usage_: Text in welcome section

##### Body Text

```css
BodyText: {
    fontSize: typeSizes[7],            // 13px
    lineHeight: typeLineHeight[7],     // 18px
    fontFamily: fontFamilies.body,     // Helvetica Neue
    fontWeight: fontWeights.regular,   // 400
}
```

_Usage_: Regular body text

##### Small Text

```css
SmallText: {
    fontSize: typeSizes[8],            // 12px
    lineHeight: typeLineHeight[8],     // 18px
    fontFamily: fontFamilies.body,     // Helvetica Neue
    fontWeight: fontWeights.regular,   // 400
}
```

_Usage_: language

##### Smaller Text

```css
SmallerText: {
    fontSize: typeSizes[9],            // 11px
    lineHeight: typeLineHeight[9],     // 18px
    fontFamily: fontFamilies.body,     // Helvetica Neue
    fontWeight: fontWeights.regular,   // 400
}
```

_Usage_: sidebar text

### Different colors

##### Body Text Secondary

```css
BodyTextSecondary: {
    color: colors.blackalpha500, //(0,0,0,0.52) = #7a7a7a
    fontSize: typeSizes[7], // 13px
    lineHeight: typeLineHeight[7], // 18px
    fontFamily: fontFamilies.body, // Helvetica Neue
    fontWeight: fontWeights.regular, // 400
}
```

_Usage_: introductions, tips.  
_Notes_: This color is very close to \#797979 used in file tree text, to be replaced.

##### Body Text Tertiary

```css
BodyTextTertiary: {
    color: colors.gray500, //#9b9b9b
    fontSize: typeSizes[7], // 13px
    lineHeight: typeLineHeight[7], // 18px
    fontFamily: fontFamilies.body, // Helvetica Neue
    fontWeight: fontWeights.regular, // 400
}
```

_Usage_: Notebook menu item

##### Title Text Secondary

```css
TitleSecondary: {
    color: colors.gray500,             // #9b9b9b
    fontSize: typeSizes[3],            // 22px
    lineHeight: typeLineHeight[3],     // 32px
    fontFamily: fontFamilies.body,     // Helvetica Neue
    fontWeight: fontWeights.regular,   // 400    
}
```

_Usage_: section title in welcome page, e.g., Featured Notebooks, and What's New.



