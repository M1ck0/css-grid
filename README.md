# CSS Grid

### Intro

CSS Grid is lightweight grid, not a `css` framework. You can't use this to style
your elements on page. You can use this if you want to create responsive layout
for your content.
It uses CSS `grid` feature, hence the name of this package (if I can call it package).

### Why `grid` and not `flex`?

`Grid` is a really powerfull feature in CSS and it should be used for creating
page layouts because it take so much work of your back, especially when it
comes to responsive layouts.

If you need to support IE browsers then this package is not for you. `Grid` does
work in IE but with very limited support and not all features are available.
You can see support for `grid` on [caniuse.com](https://caniuse.com/?search=grid)

Content automatically scales, and all columns will be stacked,
one above another, when viewing on smaller devices.

### What is `scss` file for?

I use `scss` to write this code because it gives 'super powers' to `css` that helps you in writing code.

If you want to fork this repository and extend it on your own or you want to contribute to this project here are instruction on
how to get started.

1. Clone this repo
2. run `npm install`
3. run `npm run watch`
4. edit `style.scss` file
5. run `npm run build`

This will install necessary package that is required for compiling `scss` code to pure `css` code.

Command `npm run watch` is used to compile `style.scss` to `css-grid.css`. It is triggered on every code change so you can include
`css-grid.css` in your project and see all the changes live.

After you're done, command `npm run build` compiles `style.scss` to `css-grid.min.css` which should be used in production as it strips all spaces,
empty lines and comments for a smaller file size. You will also get `css-grid.min.css.map` which will help you in debugging `css`.

You can find all `css` files in `css` directory in the root of this project.
