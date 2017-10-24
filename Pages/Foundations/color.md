# Colors

**When to use**

* Colors have a semantic value, e.g., green for success, blue for action and info, red for danger or error, and yellow for warning.
* Neutral colors \(white, gray, and black\) is used extensively in the product for text, border and background.
* Color usage for foreground and background should meet sufficient [contrast radio](https://leaverou.github.io/contrast-ratio/) \(minimum 3:1\) to ensure accessibility. 

**Styles**

* **For designer**, use only the following colors in the system. If any color is missing, add it in color.less file. 
* **For an engineer**, ideally you do not need to define color variables, they should be defined in the components.

```less
// All color values
@black: #000000;
@white: #ffffff;

@white-alpha-50: rgba(255, 255, 255, 0.05);
@white-alpha-100: rgba(255, 255, 255, 0.12);
@white-alpha-500: rgba(255, 255, 255, 0.5);

@black-alpha-800: rgba(0, 0, 0, 0.80); // #333333
@black-alpha-700: rgba(0, 0, 0, 0.70); // #4c4c4c
@black-alpha-500: rgba(0, 0, 0, 0.52); // #7a7a7a
@black-alpha-300: rgba(0, 0, 0, 0.34); // #a8a8a8
@black-alpha-200: rgba(0, 0, 0, 0.25); // #bfbfbf
@black-alpha-100: rgba(0, 0, 0, 0.12); // #e0e0e0
@black-alpha-50: rgba(252, 252, 250, 0.8); //#fcfcfb

@gray-900: #272727; // tooltip bg, banner bg
@gray-800: #333333; // primary text
@gray-700: #464644; // sidebar bg - rgb(70, 70, 68)
@gray-600: #797979; // secondary text (file tree)
@gray-500: #9b9b9b; // tertiary text (notebook menu item, welcome section title, github)
@gray-400: #cccccc; // dark border
@gray-300: #dddddd; // table border
@gray-200: #eeeeee; // light bg
@gray-150: #e6e8ea; // light border
@gray-100: #f5f5f5; // lighter bg
@gray-50:  #fafafa; // lightest bg

@blue-200: #64c3ff; // rgba(100,195,255)
@blue-500: #258bd2; // rgba(37, 139, 210, 1.0)
@blue-600: #217dbc;
@blue-700: #1b69a0; // rgb(27, 105, 160)

@blue-green-100: #1CA0C2; // branding and links
@blue-green-200: darken(#1CA0C2, 10%);

@green-100: #ecfdec;
@green-200: #d6e9c6;
@green-400: #10b36b;
@green-500: #16b169;
@green-600: #2AA198;
@green-700: #468847;

@red-100: #ffecec;
@red-200: #f05e57; // TODO(joy): replace #ff4450
@red-500: #db1905; // TODO(joy): replace #da4f49
@red-600: #d0011b;
@red-700: #b63e2b; // TODO(joy): replace #bd362f

@yellow-000: #ffff00;
@yellow-100: #f9edbe;
@yellow-400: #f79f10;
@yellow-500: #fdbc40;
@yellow-600: #f0c36d;
@yellow-700: #b37900;

@orange-500: #ff5224;
@orange-700: #ed770e;
@orange-800: #ff961d;

@purple-500: #9D3672;
```



