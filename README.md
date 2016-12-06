# Scratch Helpers
Helper classes for scratch framework. They use Scratch as a base. It's purpose of using is to write them inline in HTML for just easy markup.

### Color helper classes:

### Typography helper classes:

### Other helper classes:

- **align** - CSS `text-align` shortcut.
  -  `align-left`
  -  `align-center`
  -  `align-right`
- **flex** - CSS `flexbox` shortcuts.
  - `flex-center` - vertical and horizontal centering (affects on a child element).
    - `.flex-center-x` - horizontal centering.
    - `.flex-center-y` - vertical centering.
  - `.flex-stretch` - stretches child elements.
- **position** - CSS `position` shortcuts.
  - `.position-absolute`
  - `.position-relative`
  - `.position-static`
- **size** - shortcuts for easy sizing.
  - `.full-size` - full width and height dependent on parent container (`100%` with `vh` and `vw` fallbacks).
  - `.full-width` - full width of parent container.
  - `.full-height` - full height of parent container.
  - `.full-viewport-size` - full width and height dependent document size (using `vh` and `vw` with percent fallbacks).
  - `.full-viewport-width` - full width of document.
  - `.full-viewport-height` - full height of document.
- **transition** - CSS `transition` shortcuts.
  - `.transition` - default transition duration comes from Scratch config.
    - `.shorter` - shortest duration from the set.
    - `.short` - short duration from the set.
    - `.long` - long duration from the set.
    - `.longer` - longest duration from the set.
  - `.transition.delay` - default transition delay comes from Scratch config.
    - `.shorter` - shortest delay from the set.
    - `.short` - short delay from the set.
    - `.long` - long delay from the set.
    - `.longer` - longest delay from the set.


For more complex UI components you can check `Scratch UI Library`.
