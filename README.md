# Scratch Helpers
Helper classes for scratch framework. They use Scratch as a base. It's purpose of using is to write them inline in HTML for just easy markup. 

[![Gitter](https://img.shields.io/gitter/room/nwjs/nw.js.svg)](https://gitter.im/scratch-css/helpers)
[![npm (scoped)](https://img.shields.io/npm/v/@nikoloza/scratch-helpers.svg)](https://www.npmjs.com/package/@nikoloza/scratch-helpers)
[![David](https://img.shields.io/david/scratch-css/helpers.svg)](https://www.npmjs.com/package/@nikoloza/scratch-helpers)

## API reference:

### Color helper classes:
We can use them instead of `{color-name}` placeholder below, and we'll be able to use it inline in HTML to give color and background color to any element.

##### Brand colors:
- `.primary`
- `.secondary`
- `.tertiary`
- `.quaternary`
- `.quinary`

##### State colors:
- `.color-success`
- `.color-warning`
- `.color-info`
- `.color-error`

##### Social network colors:
- `.color-facebook`
- `.color-twitter`
- `.color-google`
- `.color-youtube`
- `.color-vimeo`
- `.color-rss`
- `.color-pinterest`

Use `.color-` prefix for those, to not to be confused with naming conflicts.

##### Table reference:

Let's use `{color-name}` as a placeholder for this table.

| Name                                 | Color                      | Background                 |
|---                                   |---                         |---                         |
| `.{color-name}`                      | `--{color-name}-inverse`   | `--{color-name}`           |
| `.{color-name}-contrast`             | `--{color-name}`           | `--{color-name}-contrast`  |
| `.{color-name}-color`                | `--{color-name}`           |                            |
| `.{color-name}-color-contrast`       | `--{color-name}-contrast`  |                            |
| `.{color-name}-background`           |                            | `--{color-name}`           |
| `.{color-name}-background-contrast`  |                            | `--{color-name}-contrast`  |

For example, `{color-name}` is `primary`, `--primary` itself is green and contrast color for it - `--primary-contrast` is white. As we see in the table, We can use `.primary` class to apply white color on the green background. `.primary-contrast` to opposite, like green on white. `.primary-background` for applying only green background and etc.

Don't get confused about color helpers starting with `.color-` prefix. As for only color usage, it can repeat `color` word like `.color-facebook-color-inverse`. It's the same structure, just starts with that prefix.

--

### Typography helper classes:

#### Families by priority
- `.font-family-primary`
- `.font-family-secondary`
- `.font-family-tertiary`
- `.font-family-quaternary`

#### Families by type
Also, families can be divided by type, as they may have `serif`, `sans-serif` or `monospace` options.

- **Sans Serif**
  - `.font-family-sans-serif-primary`
  - `.font-family-sans-serif-secondary`

- **Serif**
  - `.font-family-serif-primary`
  - `.font-family-serif-secondary`

- **Monospace** *(using of this is very rare, so I don't think we need priorities)*
  - `.font-family-monospace`

#### Font sizes
- `.font-size-h1`
- `.font-size-h2`
- `.font-size-h3`
- `.font-size-h4`
- `.font-size-h5`
- `.font-size-h6`
- `.font-size-h7`
- `.font-size-h8`
- `.font-size-h9`
- `.font-size-h10`

#### Font weight
- `.font-slim`
- `.font-light`
- `.font-regular`
- `.font-semibold`
- `.font-bold`
- `.font-extrabold`

#### Text transform
- `.text-transform-reset`
- `.text-uppercase`
- `.text-lowercase`
- `.text-capitalize`

`.text-` prefix applies here, since it just matches CSS naming.

--

### Other helper classes for CSS shortcuts:

- Align
  -  `.align-left`
  -  `.align-center`
  -  `.align-right`

- Flexbox
  - `.flex-center` - vertical and horizontal centering (affects on a child element).
  - `.flex-center-x` - horizontal centering.
  - `.flex-center-y` - vertical centering.
  - `.flex-stretch` - stretches child elements.
  - Directions
    - `.flex-row`
    - `.flex-row-reverse`
    - `.flex-column`
    - `.flex-column-reverse`

- Position
  - `.position-absolute`
  - `.position-relative`
  - `.position-static`

- Display
  - `.display-flex`
  - `.display-inline-flex`
  - `.display-none`
  - `.display-block`
  - `.display-inline`
  - `.display-inline-block`
  - `.display-table`
  - `.display-table-row`
  - `.display-table-cell`

- Sizing
  - `.full-size` - full width and height dependent on parent container (`100%` with `vh` and `vw` fallbacks).
  - `.full-width`
  - `.full-height`
  - `.full-viewport-size` - full width and height dependent on document size (using `vh` and `vw` with percent fallbacks).
  - `.full-viewport-width`
  - `.full-viewport-height`

- Transition
  - `.transition` - default duration, which is defined in Scratch config.
    - `.shorter`
    - `.short`
    - `.long`
    - `.longer`
  - `.transition.delay` - default delay, which is defined in Scratch config.
    - `.delay-shorter`
    - `.delay-short`
    - `.delay-long`
    - `.delay-longer`


For more complex UI components you can check [Scratch UI Library](https://github.com/scratch-css/ui). For animations, check [Animations Library](https://github.com/scratch-css/animations).

--

### Using examples:

    <main class="flex-center | full-viewport-size | position-absolute">

      <article class="primary-background-inverse">
        <h1 class="text-uppercase">Title</h1>
        <p class="margin-bottom-gutter-large">Lorem ipsum dolor sit amet</p>
        <a class="primary-color | text-underline">Learn More</a>
      </article>

    </main>

