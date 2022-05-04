# Text formatting
## font-family
'_font-family_' defines type of font.
```css
.arial {
    font-family: Arial, Helvetica, sans-serif;
}
```
Therea are next types of font:
- __serif__
- __sans-serif__
- __cursive__
- __monospace__
- __fantasy__

## font-size
'_font-size_' defines size of font.
```css
.fontsize {
    font-size: 30px;
}
```

## font-style
```css
.normal {
    font-style: normal; /*normal text*/
}

.italic {
    font-style: italic; /*italic text*/
}

.oblique {
    font-style: oblique; /*oblique text*/
}
```
For some fonts there aren't difference between __oblique__ and __italic__

## font-weight
```css
.weight {
    font-weight: 700; /*bold*/
}
```
The most common values:
- 100 - thin
- 300 - lite
- 400 - normal
- 500 - medium
- 600 - semibold
- 700 - bold
- 900 - black

## color
```css
.colored1 {
    color: red;
}

.colored2 {
    color: #ff0000;
}

.colored3 {
    color: rgb(255, 0, 0)
}
```

## text-align
```css
.left {
    text-align: left; /*by default*/
}

.right {
    text-align: right;
}

.center {
    text-align: center;
}

.justify {
    text-align: justify;
}
```

## text-decoration
```css
.underlined {
    text-decoration: underline;
}

.overlined {
    text-decoration: overline;
}

.line-through {
    text-decoration: line-through;
}

.underalined-and-overlined {
    text-decoration: underlined, overlined;
}

.none {
    text-decoration: none
}
```

## text-shadow
Property _text-shadow_:
```
text-shadow: horizontal_offset vertical_offset size color
```
```css
.shadow {
    text-shadow: 1px 1px 1px #000000
}
```

## text-transform
```css
.none {
    text-transform: none; /*Not modified case*/
}

.lowercase {
    text-transform: lowercase;
}

.uppercase {
    text-transform: uppercase;
}

.capitalize {
    text-transform: capitalize;
}
```
Value '__capitalize__' make the first symbol of every word uppercase.
It doesn't modify case of other symbols.

## text-indent
```css
.indent {
    text-indent: 50px;
}
```

## letter-spacing
```css
.letterspacing {
    letter-spacing: 5px;
}
```

## word-spacing
```css
.wordspacing {
    word-spacing: 5px;
}
```

## line-height
```css
.lineheight {
    line-height: 50px;
}
```

## white-space
```css
.wrap {
    white-space: normal; /*Wrap text. By default*/
}

.nowrap {
    white-space: nowrap;
}
```
