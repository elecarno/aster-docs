---
title: High Contrast
layout: default
has_toc: true
parent: Default Themes
---


- TOC
{:toc}

# High Contrast Theme
**File name:** `highcon.css`

High Contrast is one of the default themes within the [Aster Web](../../index.md) project. It is designed to aid in usage of the client for those with visual impairments. This page contains an annotated version of the theme's CSS for example purposes. The original file can be found [here](https://github.com/Jachdich/aster-web/blob/main/src/assets/themes/highcon.css).

## Variables
The theme is based on using only two colours, as such the colour variables have been set accordingly so that all of the background or panel colours are pure black and all of the main visual elements such as text will be pure white. This does not work to create a high contrast theme on its own as many of Aster Web's components are borderless however it is a good starting point for the theme.
```css
:root {
  /* colours */
  --panel-0: black;
  --panel-1: black;
  --panel-2: black;
  --panel-3: black;

  --accent-1-light: white;
  --accent-1-dark: black;
  --accent-2: white;

  --white-1: white;

  --text-dark: black;
  --text-gray: white;
}
```

## HTML Tag Styles
This section contains the style overrides for various HTML tags which are used commonly throughout Aster. It primarily concerns the interactive elements (`button` and `select`) and ensures that they have visible borders in their default state and have an easily recognisable hover state by fully inverting the colours used. Note the usage of `!important` to ensure that these styles override any default styles that may be present within the Aster Web app.

```css
button {
  border: white 2px solid !important;
  transition: 0.3s !important;
}
button:hover {
  background-color: white !important;
  color: black !important;
}
select{
  border: white 2px solid !important;
  transition: 0.3s !important;
}
select:hover {
  background-color: white !important;
  color: black !important;
}
hr {
  background-color: white !important;
  height: 2px !important;
}
```

## Login Page
This section contains the styles for the [PageLogin](../../components/pagelogin) svelte component. Despite already defining a hover state for the `button` tag, it has been specifically defined again here for the Login Page buttons as Aster Web already contains unique styles for these buttons. This is to ensure that the buttons are properly styled for the High Contrast theme. Other themes may use the `.btn-login` class identifier to add a unique flair to the Login Page buttons.

```css
/* PageLogin */
.pan-login {
  border: white 2px solid !important;
  border-bottom: white 2px solid !important;
}
.btn-login:hover {
  background-color: black !important;
  border: white 2px solid !important;
  color: white !important;
}
.con-login-input input {
  border: white 2px solid !important;
}
```

## Remaining Styles
The remaining style overrides follow the same general philosophy as those above. The unique features of the theme are applied anywhere that they are needed in order to override any clashing unique styles within the Aster Web app. It is important to note that for styling the various Dialogs within Aster Web, a theme should start with defining styles of the [Dialog](../../components/dialog) component itself as this though it is not used on its own it is the basis for all other Dialogs within the app and thus it's styles will apply accordingly.

```css
/* PageMain */
.btn-addserver,
.btn-account {
  border: white 2px solid !important;
}
.btn-aster:hover {
  border: white 2px solid !important;
}

/* ServerListButton */
.btn-server {
  border: white 2px solid !important;
}

/* PanelServerView */
.con-server-area {
  border-left: white 2px solid !important;
  border-bottom: white 2px solid !important;
}
.pan-server-messages {
  border-left: white 2px solid !important;
}
.inp-message {
  border: white 2px solid !important;
}

/* ChannelListButton */
.btn-channel {
  background-color: black !important;
  border: black 2px solid !important;
  border-bottom: white 2px solid !important;
  color: white !important;
  margin-bottom: 10px !important;
}
.btn-channel:hover {
  background-color: white !important;
  color: black !important;
}

/* ServerMessage */
.con-message:hover {
  border-left: white 2px solid !important;
  border-right: white 2px solid !important;
}

/* Dialog */
.pan-bg-darken {
  background-color: rgba(0, 0, 0, 0.8) !important;
}
.pan-dialog {
  border: white 2px solid !important;
}
.pan-dialog input {
  border: white 2px solid !important;
}
.pan-dialog label span{
  border: white 2px solid !important;
}
```
