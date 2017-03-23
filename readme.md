# Browser Technologies

## Details & Summary

[Live demo](https://rijkvanzanten.github.io/minor-bt/details-summary.html)

The `<details>` element can be used as a disclosure widget from which the user can retrieve additional information. This pattern is also known as a accordion.

### Sources
-  [MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/details)
-  [html5doctor](http://html5doctor.com/the-details-and-summary-elements/)

### Supports
-  [ ] IE
-  [ ] Edge
-  [x] Firefox (49+)
-  [x] Chrome (49+)
-  [x] Safari (6+)
-  [x] Opera (15+)
-  [x] iOS Safari (6.1+)
-  [ ] Opera Mini
-  [x] Android Browser (4+)
-  [x] Chrome for Android

### Fallback
Browser which don't support the elements will ignore them and fall back to the contents inside the elements.


## Context Menu

[Live demo](https://rijkvanzanten.github.io/minor-bt/context-menu.html)

The `<menu>` and `<menuitem>` elements can be used in combination with the `context` type attribute to provide extra contextual options in the right-click-menu.

### Sources
-  [SitePoint](https://www.sitepoint.com/whats-new-in-html-5-1/)
-  [MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/menu)

### Supports
-  [ ] IE
-  [ ] Edge
-  [x] Firefox (8+) (Partial)
-  [ ] Chrome (41+) (Flag)
-  [ ] Safari
-  [ ] Opera (35+) (Flag)
-  [ ] iOS Safari
-  [ ] Opera Mini
-  [ ] Android Browser
-  [ ] Chrome for Android

### Fallback
The contextual options should at all times be optional extras next to the regular controls. It isn't really possible to mimic the same functionality without overriding the right-click event and adding your own custom interface element (which is a big no-no usability and accessibility wise is you ask me).
