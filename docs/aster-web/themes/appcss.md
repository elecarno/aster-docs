---
title: app.css Styles
layout: default
has_toc: false
parent: CSS Reference
---

# Aster Web App Styles
This page contains the styles present within the `app.css` file of [Aster Web](../index.md). It does not include the variables, which can be found on the page [CSS Reference](./css-reference.md).

```css
/* base styles -------------------------------------------------------------- */
* {
  font-family: var(--font-body-sans);
}

/* body */
body, 
html {
  height: 100%;
  margin: 0;
  padding: 0;
}
body {
  background-color: var(--panel-0);
  color: var(--white-1);
}
#app,
 main {
   height: 100%;
  width: 100%;
}

/* interactables */
input, textarea, button {
    color: var(--white-1);
    background-color: var(--panel-1);

    border: 1px none;
    border-radius: var(--radius-3);
}
button, select {
  cursor: pointer;
}
button:hover {
  background-color: var(--panel-0);
}
input:focus {
  outline: none;
}

/* global ------------------------------------------------------------------- */
hr {
  height: 3px; 
  width: 90%; 
  
  margin: 0 auto; 
  margin-bottom: 16px; 
  
  background-color: var(--panel-3); 
  
  border: none
}

.pixel-img {
  image-rendering: pixelated;
  image-rendering: crisp-edges;
  image-rendering: -moz-crisp-edges;
  shape-rendering: crispEdges;
}

a:link {
  color: var(--accent-2);
}
a:visited {
  color: var(--accent-2);
}

/* dialogs ------------------------------------------------------------------ */
.con-dialog-row {
  display: flex;
  flex-direction: row;
  justify-content: stretch;
  align-items: center;
  text-align: center;
  
  font-size: var(--font-size-body);
}

/* used for full width text in dialogs */
.con-dialog-row p {
  width: 100%;
  margin: 0;
}

/* used for input labels */
.con-dialog-row span {
  width: 40%;
  
  margin: 0;
  
  /* padding to make the text look aligned
  with the left edge because the buttons
  below have rounded corners */
  padding-left: 3px;
  
  text-align: left;
}

.con-dialog-row input {
  height: 30px;
  width: 60%;
  
  padding-left: 10px;
}

.con-dialog-row button {
  height: 30px;
  width: 100%;
}
```