# Box model
## box-sizing
Change an algorithm of calculating '_width_' and '_height_'.
Values:
- '__content-box__' - '_width_' and '_height_' doesn't include padding, border and margin
- '__padding-box__' - '_width_' and '_height_' include padding, but doesn't include border and margin
- '__border-box__' - '_width_' and '_height_' include padding and border, but doesn't include margin
It's the inherited property. 

## padding
Defines indents from content to border.
```css
.padding4 {
    padding: 10px 15px 20px 5px; /*top right bottom left*/
}

.padding3 {
    padding: 10px 15px 20px; /*top left-right bottom*/
}

.padding2 {
    padding: 10px 15px; /*top-bottom left-right*/
}

.padding1 {
    padding: 10px; /*all*/
}
```
It isn't inherited property.
Top and bottom indents doesn't apply to inline elements.

## margin
Defines outer indents of block.
Using of this property is similar to '_padding_'.
However, margin can be negative and it is useful in practice.
```css
.negative {
    margin: 10px -10px; /*block overflow parent 10px in left and right sides*/
}
```
It isn't inherited property.
Top and bottom indents doesn't apply to inline elements.

## width, min-width, max-width
'_width_' is a width of block.
'_min-width_' and '_max-width_' are constraints for '_width_'.
__Note:__ '_min-width_' and '_max-width_' are important in adaptive markup.
They aren't inherited property.

## height, min-height, max-height
'height' is a height of block.
'min-height' and 'max-height' are constraints for '_height_'.
__Warning:__ You must be careful with properties 'height' and 'max-height'. If content height is more than these properties, there will be overflow.

## overflow
Defines behaviour of a block when it's content overflow sizes of the block size.
```css
.visible {
    overflow: visible; /*overflowed part is visible*/
}

.hidden {
    overflow: visible; /*overflowed part is hidden*/
}

.scroll {
    overflow: scroll; /*block has scrolls, even it doesn't need them*/
}

.auto {
    overflow: auto; /*scrolls appeared when they are necessary*/
    /*the most recommended option*/
}
```

## display
- block - an element get all width of parent. Properties such as '_width_' work. 
- inline - an element get only it's width from parent. Properties such as 'height' don't work.
- inline-block - an element get only it's width from parent. Properties such as 'width' work.
```css
.block {
    display: block; 
}  

.inline { 
    display: inline;
}

.inline-bloc {
    display: inline-block;
}
```