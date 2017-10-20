# Link

##### Text Link

```css
BodyTextLink: {
    color: colors.@bluegreen100, //Branding #1CA0C2
    fontSize: typeSizes[7], // 13px
    lineHeight: typeLineHeight[7], // 18px
    fontFamily: fontFamilies.body, // Helvetica Neue
    fontWeight: fontWeights.regular, // 400
}
```

_Usage_: Featured notebook links, latest release notes.

##### Text Link Hover

```css
BodyTextLinkHover: {
    color: colors.@bluegreen200, //darken(#1CA0C2, 10%);
    fontSize: typeSizes[7], // 13px
    lineHeight: typeLineHeight[7], // 18px
    fontFamily: fontFamilies.body, // Helvetica Neue
    fontWeight: fontWeights.regular, // 400
}
```

_Usage_: Hover state for featured notebook links, latest release notes.

##### **Icon and text **

```css
// todo: replace the pseudo code with right format

IconText-homeview:{
    icon: colors.@bluegreen100,
    text: colors.gray800, //#333

    hover:{
        textcolor: colors.@bluegreen200, // #333
        text-decoration: underline;
    }

    disable:{
        opacity:disabledOpacity, 
    }
}

IconText-filetree:{
    color:colors.gray600, //#797979   

    hover:{
        background-color: colors.gray100, 
    }
    selected:{
        background-color: colors.gray200,
    }

}

IconText-notebookMenu:{
    color:color.gray500,  //to be replaced    
    hover:{
        background-color: colors.gray600, 
    }
    disabled:{
        opacity:disabledOpacity,
    }

}
```

_Usage_: File tree item, notebook menu, home view actions

