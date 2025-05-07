# slight.css

**slight.css** is an incredibly simple CSS stylesheet that adds some _slight_ enhancements on top of the default user agent stylesheet.

it aims to provide a more pleasant reading experience while relying mostly on native browser styles. things such as background and text colors are chosen by the browser.

this can be used as a good baseline for any web project, or as-is for a super barebones website/blog.

## how do i use it?

### html import

place this somewhere in your `<head>`:

```
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@intergrav/slight.css@1">
```

### css import

place this somewhere in your stylesheet:

```
@import url(https://cdn.jsdelivr.net/npm/@intergrav/slight.css@1);
```

### npm package

run this in your terminal, **replace with the proper command**:

```
[npm/yarn/pnpm/bun] add @intergrav/slight.css
```

## what exactly does it change?

1.  automatically adjusts the color scheme based on system preferences
2.  uses the default system sans-serif/monospace fonts
3.  sets a maximum width for the body content on widescreen viewports (reverted when printing)
4.  increases line height and changes tab size
5.  adds borders and padding to table elements for better spacing and clarity
6.  adds a border to inline code and code blocks for better readability
7.  makes blockquotes look a bit nicer with a border and padding
8.  displays lists in nav horizontally when placed in header

keep in mind that mostly relying on the user agent stylesheet means that things could possibly look different on other browsers. for certain projects, this may matter, and you might want to look into using a CSS reset/normalize stylesheet such as [modern-normalize](https://github.com/sindresorhus/modern-normalize).

## can i see what it looks like?

yes! there is a demo available at [slightcss.devins.page](https://slightcss.devins.page). keep in mind that it may look different depending on the browser you use.

## difference between this and dev.css?

i maintain and use both, but this is a much more simple alternative to dev.css that mainly focuses on improving default user agent stylesheets rather than having a full custom set of styles. slight.css is more limited as it has less built-in element styles and doesn't have custom theme support (although you can apply your own stylesheets on top). it may also be less consistent across browsers.
