# CSS Grid

### Intro

CSS grid is a simple library that gives you an ability to create responsive layouts without thinking too much about it. It uses grid feature from CSS to create layouts for modern browsers.
This is not Bootstrap, Tailwind or something similar. You can't use this to create buttons, cards, modals, etc.

For now this library is very small (unminified version has 59 lines of code), but you can create some interesting layouts with it.
Soon I'll be adding some presets for layouts. This means that you'll be able to create nice looking galleries and layouts with only one class.

I was using Bootstrap for a long time and realized that I mostly use it because I can easily create responsive layouts, which means that other parts of it are unused, so that's why I decided to create this.
I wanted to do for myself, but then I decided to open-source it because someone might find it useful or even contribute to it.

---

### Why `grid` and not `flex`?

`grid` is a really powerful feature in CSS, and it should be used for creating
page layouts because it takes so much work off your back, especially when it
comes to responsive layouts.

If you need to support IE browsers then this package is not for you. `grid` does
work in IE but with very limited support, and not all features are available.
You can see support for `grid` on [caniuse.com](https://caniuse.com/?search=grid)

Content automatically scales, and all columns will be stacked,
one above another, when viewing on smaller devices.

---

### What is `scss` file for?

I use `scss` to write this code because it gives 'superpowers' to `css`, and helps me in writing code faster.

If you want to fork this repository and extend it on your own, or you want to contribute to this project,
here are instructions on how to get started with it.

1. Clone this repo
2. run `npm install`
3. run `npm run watch`
4. edit `css-grid.scss` file
5. run `npm run build`

This will install necessary package that is required for compiling `scss` code to pure `css` code.

Command `npm run watch` is used to compile `css-grid.scss` to `css-grid.css`. It is triggered on every
code in `css-grid.scss` and updates `css-grid.css` with the latest changes, so you can include `css-grid.css`
in your project and see all the changes live.

After you're done, command `npm run build` compiles `css-grid.scss` to `css-grid.min.css` which should be used in production as it strips all spaces,
empty lines and comments for a smaller file size. You will also get `css-grid.min.css.map` which will help you in debugging `css`.

You can find all `css` files in `css` directory in the root of this project.

---

### ToDo

- [ ] Add features in README
- [ ] Create simple landing page for this repo
- [ ] Add more examples
- [ ] Add `postcss` when compiling code for better support
