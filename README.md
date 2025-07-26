# slight.css

**slight.css** is an incredibly simple CSS stylesheet that adds some _slight_ enhancements on top of the default user agent stylesheet.

it aims to provide a more pleasant reading experience while relying mostly on native browser styles. things such as background and text colors are chosen by the browser.

this can be used as a good baseline for any web project, or as-is for a super barebones website/blog.

## how do i use it?

### html import

place this somewhere in your `<head>`:

```
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@intergrav/slight.css@2">
```

### css import

place this somewhere in your stylesheet:

```
@import url(https://cdn.jsdelivr.net/npm/@intergrav/slight.css@2);
```

### npm package

run this in your terminal, **replace with the proper command**:

```
[npm/yarn/pnpm/bun] add @intergrav/slight.css
```

## what exactly does it change?

1. automatically adjusts the color scheme based on system preferences
2. uses the default system sans-serif/monospace fonts
3. sets a maximum width for the body content on widescreen viewports
4. increases line height and changes tab size
5. opt-in styles for elements in containers with `prose` class:
   1. sets 100% maximum width for images, videos, and iframes
   2. adds a background to inline code and code blocks for better readability
   3. adds borders and padding to table elements for better spacing and clarity
   4. makes blockquotes look a bit nicer with a border and padding

keep in mind that this is not a CSS reset or normalization stylesheet. it simply adds some better defaults with the aim of being as minimal as possible. if you need a normalization stylesheet, i recommend using [modern-normalize](https://github.com/sindresorhus/modern-normalize).

## prose elements

slight.css offers built-in styles to beautify certain elements, such as blockquotes, tables, code, pre, and more. these styles are **opt-in**, and to use them, you have to apply the `prose` class to a container that wraps your content, such as a `body`, `main`, or `div`. you can see the demo's [index.html](https://github.com/intergrav/slight.css/blob/main/index.html) for an example of it's usage.

## can i see what it looks like?

yes! there is a demo available at [slightcss.devins.page](https://slightcss.devins.page). keep in mind that it may look different depending on the browser you use.

## difference between this and dev.css?

i maintain and use both, but this is a much more simple alternative to [dev.css](https://devcss.devins.page) that mainly focuses on improving default user agent stylesheets rather than having a full custom set of styles. it doesn't have custom theme support (although you can apply your own stylesheets on top). it may also be less consistent across browsers. another difference is that dev.css is classless, while slight.css contains a `prose` class.
