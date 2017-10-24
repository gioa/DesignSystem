# Colors

**When to use**

* Colors have a semantic value, e.g., green for success, blue for action and info, red for danger or error, and yellow for warning.
* Neutral colors \(white, gray, and black\) is used extensively in the product for text, border and background.
* Color usage for foreground and background should meet sufficient [contrast radio](https://leaverou.github.io/contrast-ratio/) \(minimum 3:1\) to ensure accessibility. 

**Styles**

* **For designer**, use only the following colors in the system. If any color is missing, add it in color.less file. 
* **For an engineer**, ideally you do not need to define color variables, they should be defined in the components.

```js
const colors = {

     black: '#000000',
     white: '#ffffff',

     whitealpha50: 'rgba(255, 255, 255, 0.05)',
     whitealpha100: 'rgba(255, 255, 255, 0.12)',
     whitealpha500: 'rgba(255, 255, 255, 0.5)',

     blackalpha800: 'rgba(0, 0, 0, 0.80)', // #333333
     blackalpha700: 'rgba(0, 0, 0, 0.70)', // #4c4c4c
     blackalpha500: 'rgba(0, 0, 0, 0.52)', // #7a7a7a
     blackalpha300: 'rgba(0, 0, 0, 0.34)', // #a8a8a8
     blackalpha200: 'rgba(0, 0, 0, 0.25)', // #bfbfbf
     blackalpha100: 'rgba(0, 0, 0, 0.12)', // #e0e0e0
     blackalpha50: 'rgba(252, 252, 250, 0.8)', //#fcfcfb

     gray900: '#272727', // tooltip bg, banner bg
     gray800: '#333333', // primary text
     gray700: '#464644', // sidebar bg  rgb(70, 70, 68)
     gray600: '#797979', // secondary text (file tree)
     gray500: '#9b9b9b', // tertiary text (notebook menu item, welcome section title, github)
     gray400: '#cccccc', // dark border
     gray300: '#dddddd', // table border
     gray200: '#eeeeee', // light bg
     gray150: '#e6e8ea', // light border
     gray100: '#f5f5f5', // lighter bg
     gray50:  '#fafafa', // lightest bg

     blue200: '#64c3ff', // rgba(100,195,255)
     blue500: '#258bd2', // rgba(37, 139, 210, 1.0)
     blue600: '#217dbc',
     blue700: '#1b69a0', // rgb(27, 105, 160)

     bluegreen100: '#1CA0C2', // branding and links  

     green100: '#ecfdec',
     green200: '#d6e9c6',
     green400: '#10b36b',
     green500: '#16b169',
     green600: '#2AA198',
     green700: '#468847',

     red100: '#ffecec',
     red200: '#f05e57', // TODO(joy): replace '#ff4450
     red500: '#db1905', // TODO(joy): replace '#da4f49
     red600: '#d0011b',
     red700: '#b63e2b', // TODO(joy): replace '#bd362f

     yellow100: '#f9edbe',
     yellow400: '#f79f10',
     yellow500: '#fdbc40',
     yellow600: '#f0c36d',
     yellow700: '#b37900',

     orange500: '#ff5224',
     orange700: '#ed770e',

     purple500: '#9D3672',
}
```



