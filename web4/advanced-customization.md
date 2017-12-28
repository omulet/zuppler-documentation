# Advanced customization

> So I have a fully working Order Online page, the colors and fonts looks legit, but hey!... I won't stop here. I want to go fancy! Yes, I acknowledged and I agree that I will get dirty with some HTML and CSS. Google Chrome is my browser of choice and I use it because it comes bundled with one of the best [Developer Tools](https://developer.chrome.com/devtools) out there.

If you're not yet familiarized with the DevTools we strongly recommend you take a few moments and scratch its surface at least.

## Everything is just HTML and inline styles

The Zuppler Integration Client is powered by pure Javascript with React as the rendering engine and 'CSS in JS[^1]' technique to style the elements. We have exposed meaningful class names to most of the elements, so they can be easily targeted to override the appearance.

## Overriding styles

Let's suppose you'd like to have a shadow underneath the category names. **Right click** on the category name and chose **Inspect**. The DOM element gets highlighted In DevTools, under the Elements tab. Mine looks like this:

```html
<h2 class="z-menu-category-title" data-radium="true" style="font-size: 1em; font-family: inherit; text-align: center; margin: 0px; color: #ffffff;">Sandwiches</h2>
```

Note the class name `z-menu-category-title`, so let's write some custom CSS to add the shadow:

```css
.z-menu-category-title {
    text-shadow: 0 1px 1px rgba(0,0,0,.3);
}
```

For an extra margin, you must add a higher specificity[^2] to this rule, since the element has already provided with a margin via styles attribute.

```css
.z-menu-category-title {
    text-shadow: 0 1px 1px rgba(0,0,0,.3);
    margin: 1em !important;
}
```

It is completely up to you where you add the extra CSS. So you can either edit your site .css file, or add it inside a &lt;style&gt; tag on your HTML page, both methods absolutely fine.





[^1]: In case you're wondering why "inline styles", among many reasons... it helps us avoid lots of possible CSS conflicts.

[^2]: Read more about [CSS specificity](https://developer.mozilla.org/en-US/docs/Web/CSS/Specificity)

