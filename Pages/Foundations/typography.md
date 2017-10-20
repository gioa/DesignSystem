# Typography

### Basic variables 

##### When to use

* Use the following variables to define the text styles in the UI components.
* If any is missing, add in font.less.

##### Font family

```js
const fontFamilies = {
  display: 'Newslab',     // Branding font, used in "Welcome to Databricks"
  body: 'Helvetica Neue', // Body font, default font
  icon:'FontAwesome',     // Icon font, used for icons 
  code:'Source Code Pro', // Code font, used in Notebook cell command and result
}
```

##### Font size and line height

```js
const typeSizes      = [52, 33, 26, 22, 18, 16, 14, 13, 12, 11];
const typeLineHeight = [72, 48, 36, 32, 24, 24, 20, 18, 16, 16];
```

##### Font weight

```js
const fontWeights = {
  lighter: 200,
  light: 300,
  regular: 400,
  medium: 500,
  bold: 700,   
};
```

### Different sizes

##### Headline

```css
 Headline: {
    color: colors.blackalpha300,       // (0,0,0,0.34)
    fontSize: typeSizes[0],            // 52px
    lineHeight: typeLineHeight[0],     // 72px
    fontFamily: fontFamilies.display,  // Newslab
    fontWeight: fontWeights.regular,   // 400

}
```

_Usage_: Welcome to Databricks

##### Large Title

```css
 LargeTitle: {
    color: colors.gray800,             // #333
    fontSize: typeSizes[1],            // 33px
    lineHeight: typeLineHeight[1],     // 48px
    fontFamily: fontFamilies.body,     // Helvetica Neue
    fontWeight: fontWeights.regular,   // 400
}
```

_Usage_: Workspace Access Control \(to be deprecated\)

##### Page Title

```css
PageTitle: {
    color: colors.gray800,             // #333
    fontSize: typeSizes[2],            // 26px
    lineHeight: typeLineHeight[2],     // 36px
    fontFamily: fontFamilies.body,     // Helvetica Neue
    fontWeight: fontWeights.lighter,   // 200

}
```

_Usage_: Dialog title, Create New Cluster\(to be deprecated\)

##### Title

```css
Title: {
    color: colors.gray800,             // #333
    fontSize: typeSizes[3],            // 22px
    lineHeight: typeLineHeight[3],     // 32px
    fontFamily: fontFamilies.body,     // Helvetica Neue
    fontWeight: fontWeights.regular,   // 400    
}
```

_Usage_: Sign In to Databricks, future page titles

##### Section Title

```css
SectionTitle: {
    color: colors.gray800,             // #333
    fontSize: typeSizes[4],            // 18px
    lineHeight: typeLineHeight[4],     // 24px
    fontFamily: fontFamilies.body,     // Helvetica Neue
    fontWeight: fontWeights.regular,   // 400
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



