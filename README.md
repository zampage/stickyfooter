# Sticky Footer
A modern easy to use sticky footer mixin with minimal HTML requirements.

Example: [zampage.github.io/stickyfooter/](https://zampage.github.io/stickyfooter/)

## Usage

### SCSS
```scss
parent{
  @include stickyFooter(); //takes 2. child as footer
  @include stickyFooter('content', 'footer'); //takes your selector as footer
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
- [X] Chrome >= 57
- [X] Firefox >= 52
- [X] MS Edge >= 16
- [ ] IE - not supported
- [X] Safari >= 10.1
- [X] Opera >= 44

Notice: It is not recommended to use sticky footer on mobile.