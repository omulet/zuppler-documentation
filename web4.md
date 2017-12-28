# Web4 - Integration Instructions

The easiest way to integrate our menus is to use a default configuration, then fine tune the appearance using our ThemeRoller helper tool.

### Step 1

Create a separate HTML page and set the appropriate title, let's say "Order Online". To simplify things, you can start by duplicating one of your existing pages, like about-us.html. Or, if you're using a CMS \(e.g. Wordpress\), simply create a new page.

### Step 2

Edit this page and remove the existing content \(if present\). Only keep the usual components, like the page header with your logo, main navigation, page title, footer, etc.

Copy the following markup and paste it into your newly created page.

```html
<div id='zuppler-menu'
  data-channel-url='http://api.zuppler.com/v3/channels/demorestaurant.json'
  data-integration='site'
  data-restaurant-id='242'

  data-colors-background='#ffffff'
  data-colors-highContrast='#000000'
  data-colors-midContrast='#797979'
  data-colors-lowContrast='#c0c0c0'
  data-colors-brand='#3265d3'
  data-colors-heroBackground='#3265d3'
  data-colors-heroContrast='#FFFFFF'

  data-fonts-heading='Open Sans Condensed, helvetica, sans-serif'
  data-fonts-body='Raleway, helvetica, sans-serif'
  data-fonts-deco='Montserrat, helvetica, sans-serif'>

  <div id='zloading'>Please wait. Loading menu...</div>
</div>

<script src='//web4.zuppler.com/common.js'></script>
<script src='//web4.zuppler.com/order.js'></script>
```

_This code is based on Zuppler's Demo Restaurant._

At this point, we assume that your Zuppler Account Manager already provided you the configuration information for your real restaurant. If this is the case, make sure you replace `data-channel-url` , `data-integration` and `data-restaurant-id` with the correct values in the code above. Otherwise, you can continue with the Demo, make sure everything works fine, then simply add the real data later on.

### Step 3

Save, and visit the page using your favorite internet browser. Congrats!! 🍾🎉 You should now have a fully functional Order Online page.

However, there is a big chance you want to change the colors because the defaults doesn't really match with the look & feel of your page.  Read on to the ThemeRoller instructions.

