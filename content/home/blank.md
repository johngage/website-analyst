---
widget: blank
headless: true
design:
  # Choose how many columns the section has. Valid values: 1 or 2.
  columns: '1'

# ... Put Your Section Options Here (title etc.) ...
gallery_item:
 - album: gallery
   image: hello.jpg
   caption: gallery one
 - album: gallery
   image: https://static01.nyt.com/vi-assets/images/share/1200x675_nameplate.png
   caption: Another caption
---
{{< gallery >}}
  
{{< figure library="true" src="hello.jpg" title="Duplicate" >}}

