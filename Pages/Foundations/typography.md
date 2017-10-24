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



##### headline

```less
.headline {
    font-size: @font-size-x-large;
    line-height: @line-height-x-large;
    font-family: @newslab-font;
    color: @black-alpha-300;
}
```

_Usage_: Welcome to Databricks

##### title-large

```less
 .title-large {
    font-size: @font-size-large;
    line-height: @line-height-large;
}
```

_Usage_: Workspace Access Control \(to be deprecated\)

##### title-dialog

```less
.title-dialog {
    font-size: @font-size-h1;
    line-height: @line-height-h1;
    font-weight: @font-weight-light;
}
```

_Usage_: Dialog title, Create New Cluster\(to be deprecated\)

##### title-page

```less
.title-page {
    font-size: @font-size-h2;
    line-height: @line-height-h2;
 }
```

_Usage_: Sign In to Databricks, future page titles

##### title-section

```less
 .title-section {
    font-size: @font-size-h3;
    line-height: @line-height-h3;
 }

```

_Usage_: Sample Data, Interactive Cluster

##### text-tab

```less
.text-tab {
    font-size: @font-size-h4; 
    line-height: @line-height-h4; 
 }

```

_Usage_: Single Sign on / Admin Login

##### text-large

```less
.text-large {
    font-size: @font-size-h5;
    line-height: @line-height-h5;
}
```

_Usage_: Text in welcome section

##### text-basic

```less
.text-basic {
    font-size: @font-size-h6;
    line-height: @line-height-h6;
}
```

_Usage_: Regular body text

##### text-small

```less
.text-small {
    font-size: @font-size-small;
    line-height: @line-height-small;
}
```

_Usage_: language

##### Smaller Text

```less
.text-smaller {
    font-size: @font-size-x-small;
    line-height: @line-height-x-small;
}

```

_Usage_: sidebar text

### Different colors

| Class | Example |
| -- | -- | 
| text-secondary | <div class="text-secondary">text secondary</div> |
| homeview-section-title | <div class="homeview-section-title">What's new?</div> |
| text-error | <div class="text-error">Invalid username or password.</div> |
| text-warning | <div class="text-warning">Make sure to copy the token now. You won't be able to see it again.</div> |

##### text-secondary

```less
.text-secondary {
    .text-basic;
    color: @text-secondary-color; //(0,0,0,0.52) = #7a7a7a
}
```

_Usage_: introductions, tips.  
_Notes_: This color is very close to \#797979 used in file tree text, to be replaced.

##### homeview-section-title

```less
.homeview-section-title{
    .title-page;
    color: @text-secondary-color;
}
```

_Usage_: section title in welcome page, e.g., Featured Notebooks, and What's New.

##### .text-error 

```less
.text-error {
    .text-basic;
    color: @text-error-color;
}
```

_Usage_: Inline error messages. 

##### text-warning

```less
.text-warning {
    .text-basic;
    color: @text-warning-color; //(0,0,0,0.52) = #7a7a7a
}
```

_Usage_: Inline warning messages. 

