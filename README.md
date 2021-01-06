# Fractable <!-- omit in toc -->

A markup challenge.

---

- [Notes on approach](#notes-on-approach)
  - [`CSS` notes](#css-notes)
    - [For speed of demo development](#for-speed-of-demo-development)
    - [Not creating fallbacks for](#not-creating-fallbacks-for)
    - [Other things to look at (not done)](#other-things-to-look-at-not-done)
  - [Other comments](#other-comments)
- [Requirements](#requirements)
  - [Development tasks](#development-tasks)
  - [Bonus tasks](#bonus-tasks)
  - [Browser support](#browser-support)
- [Run the demo locally](#run-the-demo-locally)

---

# Notes on approach

## `CSS` notes

-   Using `hsl` for colours, so I can try them out
-   Media query styles can be found in one block at end of file

### For speed of demo development

-   Working in pixels
-   Not adjusting `font-size` on mobile
-   `padding`/`margin` values would be better as `rems`/`ems` depending on how design scales for smaller viewports

### Not creating fallbacks for

-   `CSS` custom properties
-   `CSS` `grid` & `flexbox`<br/>
    ... as target browsers are latest and no `IE`/`Edge`

### Other things to look at (not done)

-   Dark mode
-   _Prefers reduced motion_ setting (if more animation/movement)

## Other comments

-   Design fails accessibility contrast requirements; I have kept to colour scheme specified regardless
-   Could make site-control/navigation panel `position: sticky` or `fixed`. However, some solid `background-color` would need to be applied (this is not part of the design)
-   On the `footer` tag, I have added `ARIA` attribute `role="contentinfo"` to cover a `VoiceOver` bug; HTML validators may warn about this being unnecessary

---

# Requirements

-   Create a static web page layout that replicates the [desktop design](design/desktop-mockup.jpg) as closely as possible
-   The only image that should be used is `fractable.jpg`, everything else must be `CSS`
-   The sans-serif font used is _Avenir Next_ (present on `macOS`; use the closest visual match available on `Windows`)
-   Typefaces:
    -   sans-serif: _Avenir Next_ (present on `macOS`; use the closest visual match available on `Windows`)
    -   serif: [_Merriweather_](https://fonts.google.com/specimen/Merriweather)

And pay attention to the details!

## Development tasks

-   Ensure valid, clean code
-   Use semantic markup
-   Consider accessibility

## Bonus tasks

-   Make layout responsive, reflowing in a suitable way
-   Add something new <br/>e.g. a visual addition or effect, or something in the technical implementation

## Browser support

The final page should look the same in the latest versions of:

-   Chrome
-   Firefox
-   Safari

# Run the demo locally

1. `cd` into project location
2. Install (one-time operation)<br/>

```
npm install
# Or;
yarn install
```

3. Start the local server<br/>

```
npm run start
# Or;
yarn start
```

Runs a local server on [http://localhost:4000]().
