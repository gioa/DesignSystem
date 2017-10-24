# Link

Can link to another page or act as text-only button. Usually it is used inline using tag `<a>`. 

| Class | Example |
| -- | -- | 
| tag `a` | <div class="db"><a>Latest release notes</a></div> |
| tag `a` and `i` |  <div class="db"><a><i class="fa "></i></a></div> |
| icon-link |<div class="db"><a class="icon-link"><i class="fa "></i>Notebook</a></div> |
| icon-link link-menu|  <div class="db"><a class="icon-link link-menu"><i class="fa "></i>Run all</a></div> |


##### Link

```less
a {
    .text-basic;
    text-decoration: none;
    color: @link-text-color;

    &:focus, &:hover {
        color: @link-hover-text-color;
        text-decoration: underline;
    }

}
```

_Usage_: Featured notebook links, latest release notes.

##### Icon only

```less
a {
    i {
        color: @link-menu-color;
        
        &:focus, &:hover {
            color: @link-hover-text-color;
            text-decoration: none;
        }
    }
}
```

_Usage_: utility links on the top right: user, help, recent icons.

##### icon-link 

```less
.icon-link {
    color: @text-basic-color;

    i {
        color: @link-text-color;
        margin-right: @spacing-small;

        &:focus, &:hover {
            color: @link-hover-text-color;
            text-decoration: none;
        }

    }

    &:focus, &:hover {
        color: @link-hover-text-color;
    }
}
```

_Usage_: Icon + link on welcome page.

##### icon-link link-menu
```less
.link-menu {
    color: @link-menu-color;

    i {
        color: @link-menu-color;
    }

    &:focus, &:hover {
        color: @text-basic-color;
        text-decoration: none;
        i {
            color: @text-basic-color;
        }
    }
}
```

_Usage_: Notebook menu.  
_Notes_: To be deprecated. Should have the same hover/seleted style as file browser items in future.


