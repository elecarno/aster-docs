---
title: Themes
layout: default
has_toc: false
parent: Aster Web
nav_order: 2
---

# Themes for Aster Web
This page discusses the design and creation of themes in the [Aster Web] project.

Themes in [Aster Web] are based on overriding the default css styles within [Aster Web]. Themes are entirely contained within a single `.css` file which can be uploaded by the user to be used within their client. Custom HTML for themes is not currently supported.

<span class="fs-6">
[Default Themes](./default-themes/){: .btn .fw-700 .w100}
[CSS Reference](./css-reference){: .btn .fw-700 .w100}
</span>

## Creating a Theme for Aster Web
To create a theme for [Aster Web], simply create a `.css` file named however you wish (although likely with the name of your theme) and populate it with style overrides. This CSS file can be directly uploaded to the Aster Web client.

### Example Theme
Create a `.css` file and open it with an editor of your choice.
```
> touch example.css
> nano example.css
```

Create the `:root` style and import some of the default variables from [CSS Reference](./css-reference/). In this case we will change just the accent colours and the standard radii for our theme.
```css
/* default variables */
:root {
  --accent-1-light: #be8fd0;
  --accent-1-dark: #a776bb;
  --accent-2: #c0a0ff;

  --radius-1: 36px;
  --radius-2: 16px;
  --radius-3: 6px;
}
```

Adjust the variables accordingly. This example will make all of the radii the same and set the accent colours to be a green hue.

```css
/* adjusted variables for theme */
:root {
  --accent-1-light: #84AE92;
  --accent-1-dark: #5A827E;
  --accent-2: #B9D4AA;

  --radius-1: 4px;
  --radius-2: 4px;
  --radius-3: 4px;
}
```

Let's say however that we want to keep the border radius on the Login Page buttons. We can add the class for the buttons and override their default styles. Make sure to use `!important` to ensure that your theme's styles are used when imported into the app.
```css
.btn-login {
    border-radius: 8px;
}
```

Save the file and open the [Aster Web] client. You can now import the file and the styles inside will be applied to the app.

In order to create more complex themes with lots of styles, you can use the [CSS Reference](./css-reference/) which contains a list of all of the default CSS indentifiers and variables used within [Aster Web].

---
[Aster Web]: ../index