Style Guide
==========

# General Code
* use two spaces instead of tabs (you can set your editor to "soft tabs" for this)

# Images
* filenames all lowercase
* use three-letter extensions (jpg, not jpeg)
* append retina versions with "@2x" before the extension. Non-retina graphics should *not* include "@1x"
* name associated images with the same prefix (fathead_gb.jpg, fathead_dis.jpg, not bg_fathead.jpg, dis_fathead.jpg).

# HTML
* use html5 tags at will


# CSS
* favor clean markup over selector performance. for example, 

```css
.bs-docs-sidenav > li > a {
  display: block;
  width: 190px \9;
  margin: 0 0 -1px;
  padding: 8px 14px;
  border: 1px solid #e5e5e5;
}
.bs-docs-sidenav > li:first-child > a {
  -webkit-border-radius: 6px 6px 0 0;
     -moz-border-radius: 6px 6px 0 0;
          border-radius: 6px 6px 0 0;
}
.bs-docs-sidenav > li:last-child > a {
  -webkit-border-radius: 0 0 6px 6px;
     -moz-border-radius: 0 0 6px 6px;
          border-radius: 0 0 6px 6px;
}
```

is preferable to

```css
.bs-docs-sidenav-li-a {
  ...
}
.bs-docs-sidenav-li-first-a {
  ...
}
.bs-docs-sidenav-li-last-a {
  ...
}
```

* it's ok to use id tags when the elements are really unique
* reuse classes whenever possible.
* never add a class name unless you need to customize a style (in other words, do not add a class unless it has a reference in css or javascript)
* if possible, use cascading styles rather than adding new classes to ever element.
* ems are your friend


# Javascript
* semi-colons at the end of lines are not necessary. checkout twitter bootstraps raw js for inspiration

