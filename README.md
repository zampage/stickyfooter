# Sticky Footer
A modern easy to use sticky footer mixin with minimal HTML requirements.

Example: [zampage.github.io/stickyfooter/](https://zampage.github.io/stickyfooter/)

## Usage

`stickyFooter([string:contentSelector, string:footerSelector])`

### SCSS
```scss
parent{
  @include stickyFooter(); //takes 1. child as content and 2. child as footer
  @include stickyFooter('content'); //takes your selector as content and 2. child as footer
  @include stickyFooter('content', 'footer'); //takes your selectors content and footer
}
```

### HTML
```html
<parent>
    <content></content>
    <footer></footer>
</parent>
```

### Notice
- if applied on body the margin needs to be resetted
- you should use box-sizing: border-box; on all elements

## Browser Support
- [X] Chrome >= 21
- [X] Firefox >= 28
- [X] MS Edge - all versions
- [X] Safari >= 6.1
- [X] Opera >= 12.1
- [ ] IE - not supported

Sticky footer will automatically be ignored completely on IE. If you want to use a fallback just for IE this is the way to go:

```scss
@media all and (-ms-high-contrast: none), (-ms-high-contrast: active) {
  //some sort of fallback
  //which is not executed in other browsers
}
```