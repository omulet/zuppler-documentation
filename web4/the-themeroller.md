# The ThemeRoller

Is a little neat tool that lets you easily find the perfect colors for your menus with real time preview. To activate it, append the `?themeRoller=true` param at the and of the URL. E.g. If the current page address is [http://demo.zuppler.com/order-online-new.html](http://demo.zuppler.com/order-online-new.html) then it changes to [http://demo.zuppler.com/order-online-new.html**?themeRoller=true**](http://demo.zuppler.com/order-online-new.html?themeRoller=true).

Once the page reloads, you should see this ![](/assets/themeroller-button.png) on the right hand side bottom corner. Click to expand the tool.

![](/assets/themeroller@2x.png)

The changes you will be doing here are **NOT persistent**. So if you refresh the page they will be gone. All this tool does is to let you preview colors and fonts changes in real time and most important to generate a new integration code base on these changes.

## Colors

* [background](#background-color)
* [highContrast](#highcontrast-color)
* [midContrast](#midcontrast-color)
* [lowContrast](#lowcontrast-color)
* [brand](#brand-color)
* [heroBackground](#herobackground-color)
* [heroContrast](#herocontrast-color)

### background {#background-color}

This color should match the actual background color of your page or of the box in which the menu gets rendered.

> For best results it is very important to set this color as close as possible with **the color perceived by human eye**. One common case to pay attention is when there is a background image behind, with a semi-transparent box above. You may be tempted to use the same css color with your box, eg. white with 60% opacity, but the result won't be optimal. Use the eyedropper to pick the right color instead.

It is used by the system to generate lighter and darker shades for different components and also to set the text color for "color reversed" components, such as the cart dropdown.

### highContrast {#highcontrast-color}

As the name suggests, the High Contrast Color should have the highest contrast possible with the [background](#background-color).

> For best results set it to black or a very dark color if your background color is light \(white\). Or to white or a very light gray if your background is dark \(black\).

It is used to draw important elements, such as active menu tabs, category names, item title and prices, etc.

### midContrast {#midcontrast-color}

The Medium Contrast color should make less contrast \(than the previous\) with the background, but still be very visible. Used on regular buttons or icon buttons, menu items description, etc.

### lowContrast {#lowcontrast-color}

Should make lesser contrast with the background but still be visible. It is used on "less important" elements, such as inactive menu tabs, category descriptions, footnotes, etc.

### brand {#brand-color}

This is the "Hey, look here!!!" color. It is the color which is most relevant to your Brand Identity. It is used on "call to action" elements such as important buttons like "Checkout" or "Add to Cart", etc.

> For best results, it should be a vivid color and at the same time a color that makes a very high contrast with the background. Like blue on white bg, or yellow on black bg, etc.

### heroBackground {#herobackground-color}

The term "hero" refers and applies to menu categories that have an image associated with them on Zuppler system. These are rendered with a different style and a background image.

The Hero Background is the color to which our image will blend with a "luminosity" mode.

### heroContrast {#herocontrast-color}

This color should have the highest contrast possible with the heroBackground color. It is used to render the content inside these categories.

> heroContrast is for heroBackground just like highContrast is for background.



