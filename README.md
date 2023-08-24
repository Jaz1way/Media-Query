# Media-Query
Using Media Query to create a responsive website

### 

```css
@media(max-width: 600px){
    h1{
        font-size: 15px;
    }
}
```

* Instead of selectors, we have the `@media` keyword.
* `breakpoint`:(max-width: 600px); which means, at this particular width, anything that is less than or equal to 600px, should use this styling.

```css
/*html*/
<div></div>
------------
/*CSS*/
div{
    background-color: blue;
    height: 200px;
    width: 200px;
}

@media(max-width: 600px){
    div{
        height: 100px;
        width: 100px;
    }
}
```

* There should always be a default styling

```css
@media (min-width:600px) and (max-width: 900px){
    /*Styles for screens between 600px and 900px*/
}
```

* You can **combine** min-width and max-width

```css
@media screen(orientation: landscape){
    /*Styles for landscape orientation*/
}
```

* `screen`: Not necessary by default because it is going to apply to all screens. Purpose is to target screens or target print.
