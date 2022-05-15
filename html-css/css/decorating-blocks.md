# Decorating blocks
## border
```css
.block {
    /*border: border_width border_style color*/
    border: 1px solid #ff0000;
}
```
Common border styles:
- solid
- dotted
- dashed

## border-radius
Radius of rounding.
```css
.block {
    /*border-radius: horizontal_radius_for_all_angles / vertical_radius_for_all_angles*/
    /*order of anles: top-left top-right bottom-right bottom-left*/
    border-radius: 5px / 10px;
}
```

## box-shadow
```css
.block {
    /*box-shadow: horizontal_offset vertical_offset blur_radius spread_radius color*/
    box-shadow: 5px 5px 10px 10px red; 
}
```

## opacity
```css
.block1 {
    opacity: 0; /*Element is not visible*/
}

.block2 {
    opacity: 1; /*Not transparency*/
}
```

## visibility
Possible values:
- '__visible__'
- '__hidden__'