# Blog Starter CSS

## Getting started

First, you should install `dart sass`

```bash
npm install -g sass
```

You can compile `.scss` to `.css` with following command.

```bash
git clone https://github.com/pengu1m/starter-blog-css.git
sass main.scss ./build/min.css
# Compile main.scss
# It imports all files under 'components'
```

You can also use `--watch` or `--style=compressed` for dev and production.

## Style Concepts

- Copy the design of [Gatsby-Starter-Blog][gsb]
- No "primary color"

## Components

- Header
- Footer
- Bio
- Card
- Content
- Hr
- Page-Navigator

## Usage (BEM)

### Header

```html
<!-- header -->
<header class="header">
  <a class="header__title" href="#">Blog of apple chef</a>
</header>

<!-- header (mini title) -->
<header class="header">
  <a class="header__title--sub" href="#">Blog of apple chef</a>
</header>
```

### Footer

```html
<!-- footer -->
<footer class="footer">
  <span class="footer__copyright">© 2023, All recipe is protected</span>
  <ul class="footer__sns">
    <li>SNS name: @apple</li>
    <li>inner content of li is free</li>
  </ul>
</footer>
```

### Bio

```html
<!-- bio -->
<div class="bio">
  <img class="bio_icon" src="#" alt="#" />
  <p class="bio_description">Apple jam chef<p>
</div>
```

### Card

```html
<!-- card -->
<div class="card">
  <a class="card__title" href="#">How to make Apple Jam</a>
  <span class="card__date">1970-02-11</span>
  <p class="card__description">Let's make VEGAN apple jam!</p>
</div>
```

### Content

```html
<!-- content -->
<div class="content">
  <h1 class="content__heading">How to make Apple Jam</h1>

  <div>
    <span class="content__date">1970-02-11</span>
    <a class="content__category" href="#">#cooking/jam</a>
  </div>

  <hr class="hr"/>

  ... (and other contents)
</div>
```

### Hr

```html
<!-- hr -->
<hr class="hr" />
```

### Page-Navigator

```html
<!-- page-navigator -->
<div class="page-navigator">
  <a class="page-navigator__previous">👈</a>
  <a class="page-navigator__next">👉</a>
</div>

<!-- page-navigator (with disabled button) -->
<div class="page-navigator">
  <a class="page-navigator__previous--disabled">❌</a>
  <a class="page-navigator__next">👉</a>
</div>
```

[gsb]: https://www.gatsbyjs.com/starters/gatsbyjs/gatsby-starter-blog