
# HelixCSS

## About

HelixCSS primary goal is to give structure to your website or application and leave the design
decisions to you.

## Documentation

For the moment there are only code examples available inside the objects folders. Over time, a
detailed documentation will be made available.

## Folders & Contents

#### Settings

To help you find the variables you are looking for faster, variables have their own folder and files.
Some variable groups have abstract variables. These abstract variables are there to shorten the setup
of the element variables but are also used inside some of the objects.

#### Base

This folder addresses mostly HTML tags, but there are also a couple of classes included. Within
HelixCSS, classes that are named exactly like HTML tags are behaving just like their respective HTML
tag counter parts.

#### Objects

Objects are CSS classes that make elements act a certain way (e.g. buttons). Object utilities are
there to manipulate objects and HTML tags. Utilities generally don't overwrite each other because
each utility only modifies the smallest set of properties possible. Object mixins currently exist
purely in SCSS.

#### Library

In here are functions, mixins and variables that are useful for SCSS development. Using the CSS3
mixins rather than a tool like [auto-prefixer](https://www.npmjs.com/package/autoprefixer) allows
for compiling on the server by using tools like [scssphp](http://leafo.net/scssphp/).

## Responsive Sizing

Throughout your project, use `rem` whenever you want a size to be adaptable to whatever the
HTML's base font-size value is set to. The base font-size varies between breakpoints. This allows for
responsive typography and sizing. Take a look at the variables inside `_typograpy.scss` to change or
disable responsive sizing.

### Reminder

- [IE 9 & 10](http://caniuse.com/#search=rem) do not support `rem` units when used in the `font`
  shorthand property (the entire declaration is ignored) or when used on pseudo elements like
  `::before` & `::after`.

## Browser & OS Support

HelixCSS supports IE9+ & Android2.3+.

## Credits

HelixCSS was inspired by these fine projects:
- [BassCSS](http://www.basscss.com/)
- [Bourbon](http://bourbon.io/)
- [KiteCSS](http://hiloki.github.io/kitecss/)
- [InuitCSS 5](https://github.com/csswizardry/inuit.css)
- [InuitCSS 6](https://github.com/inuitcss/inuitcss)

## Resources

- [http://caniuse.com/](http://caniuse.com/)
- [http://www.cssfontstack.com/](http://www.cssfontstack.com/)
