# Scratch Helpers
Helper classes for scratch framework. They use Scratch as a base. It's purpose of using is to write them inline in HTML for just easy markup.

## API reference:

### Color helper classes:
- **Brand colors**
  - `.primary` - background is `--primary`, color is `--primary-inverse`
    - `.primary-inverse` - background is `--primary-inverse`, color is `--primary`
    - `.primary-color` - color is `--primary`
    - `.primary-color-inverse` - color is `--primary-inverse`
    - `.primary-background` - background is `--primary`
    - `.primary-background-inverse` - background is `--primary-inverse`
   
  - `.secondary` - background is `--secondary`, color is `--secondary-inverse`
    - `.secondary-inverse` - background is `--secondary-inverse`, color is `--secondary`
    - `.secondary-color` - color is `--secondary`
    - `.secondary-color-inverse` - color is `--secondary-inverse`
    - `.secondary-background` - background is `--secondary`
    - `.secondary-background-inverse` - background is `--secondary-inverse`
   
  - `.tertiary` - background is `--tertiary`, color is `--tertiary-inverse`
    - `.tertiary-inverse` - background is `--tertiary-inverse`, color is `--tertiary`
    - `.tertiary-color` - color is `--tertiary`
    - `.tertiary-color-inverse` - color is `--tertiary-inverse`
    - `.tertiary-background` - background is `--tertiary`
    - `.tertiary-background-inverse` - background is `--tertiary-inverse`
   
  - `.quaternary` - background is `--quaternary`, color is `--quaternary-inverse`
    - `.quaternary-inverse` - background is `--quaternary-inverse`, color is `--quaternary`
    - `.quaternary-color` - color is `--quaternary`
    - `.quaternary-color-inverse` - color is `--quaternary-inverse`
    - `.quaternary-background` - background is `--quaternary`
    - `.quaternary-background-inverse` - background is `--quaternary-inverse`
   
  - `.quinary` - background is `--quinary`, color is `--quinary-inverse`
    - `.quinary-inverse` - background is `--quinary-inverse`, color is `--quinary`
    - `.quinary-color` - color is `--quinary`
    - `.quinary-color-inverse` - color is `--quinary-inverse`
    - `.quinary-background` - background is `--quinary`
    - `.quinary-background-inverse` - background is `--quinary-inverse`
 
### Typography helper classes:

### Other helper classes:

- **align** - CSS `text-align` shortcut.
  -  `.align-left`
  -  `.align-center`
  -  `.align-right`
- **flex** - CSS `flexbox` shortcuts.
  - `.flex-center` - vertical and horizontal centering (affects on a child element).
  - `.flex-center-x` - horizontal centering.
  - `.flex-center-y` - vertical centering.
  - `.flex-stretch` - stretches child elements.
- **position** - CSS `position` shortcuts.
  - `.position-absolute`
  - `.position-relative`
  - `.position-static`
- **sizing** - shortcuts for easy sizing.
  - `.full-size` - full width and height dependent on parent container (`100%` with `vh` and `vw` fallbacks).
  - `.full-width` - full width of parent container.
  - `.full-height` - full height of parent container.
  - `.full-viewport-size` - full width and height dependent on document size (using `vh` and `vw` with percent fallbacks).
  - `.full-viewport-width` - full width of document.
  - `.full-viewport-height` - full height of document.
- **transition** - CSS `transition` shortcuts.
  - `.transition` - default transition duration comes from Scratch config.
    - `.shorter` - shortest duration from the set.
    - `.short` - short duration from the set.
    - `.long` - long duration from the set.
    - `.longer` - longest duration from the set.
  - `.transition.delay` - default transition delay comes from Scratch config.
    - `.delay-shorter` - shortest delay from the set.
    - `.delay-short` - short delay from the set.
    - `.delay-long` - long delay from the set.
    - `.delay-longer` - longest delay from the set.


For more complex UI components you can check [Scratch UI Library](https://github.com/scratch-css/ui).

## Using examples:

    <main class="flex-center | full-viewport-size | position-absolute">
      
      <article class="primary-background-inverse">
        <h1 class="text-uppercase">Title</h1>
        <p class="margin-bottom-gutter-large">Lorem ipsum dolor sit amet</p>
        <a class="primary-color | text-underline">Learn More</a>
      </article>
      
    </main>
      
