---
title: CSS Reference
layout: default
has_toc: true
parent: Themes
nav_order: 3
---

**TABLE OF CONTENTS**
- TOC
{:toc}

# Aster Web CSS Reference
This page contains an outlline of the structure of CSS styles within [Aster Web] as well as a list of the default variables used within the css.

## Style Guide
CSS styles in [Aster Web] have each been organised using a consitent order in order to aid in readability. This order is as outlined below.

```
CSS CLASS LAYOUT {
    (height & width)
    (positioning styles)
    (flex/display styles)
    (margins)
    (padding)
    (color)
    (background color)
    (border styles)
    (font-styles)
    (other)
}
```

The various CSS identifiers used throughout the project also follow a prefixing system in order to aid in clarity of purpose and make naming easier. These prefixes are as follows:
- `con-`: An invsibile container for elements. Usuaally used for positioning.
- `pan-`: A visible container for elements.
- `lab-`: (Label). Any kind of text that is used within the app.
- `btn-`: Used for interactable elements, primarily `button`s and `select`s.
- `inp-`: Used to distinguish `input`s.
- `gra-`: Used for any graphic elements, such as `img`s or `svg`s.

## Variables
Found in the file `app.css`. These variables define the colour palette of the web app, as well as standardised radii, margins, and fonts used throughout the application.

```css
:root {
  /* colours */
  --panel-0: #1e2329;
  --panel-1: #272e39;
  --panel-2: #31363F;
  --panel-3: #3c424f;

  --accent-1-light: #be8fd0;
  --accent-1-dark: #a776bb;
  /* used for links within server messages */
  --accent-2: #c0a0ff;

  /* primary text colour */
  --white-1: #d3d3d3;

  --text-dark: #1b0a24;
  --text-gray: #929292;

  /* radii & margins */
  /* intended to function well together */
  /* outer r = inner r + margin */
  --radius-1: 36px;
  --margin-1: 20px;
  --radius-2: 16px;
  --margin-2: 10px;
  --radius-3:  6px;

  /* fonts */
  --font-body-sans: "Atkinson Hyperlegible", sans-serif;
  --font-body-mono: "Red Hat Mono", monospace;

  --font-size-body: 15px;
}
```

## CSS Structure
An outline of the heirarchy of CSS styles used in [Aster Web]. The outline is based on the HTML of the app and shows the unique styles related to each [Component] and how their are ordered in the HTML. The default styles of each [Component] can be found on the [Component]'s dedicated page, each of which is linked accordingly.

### [app.css](./appcss)
```
(body html main input textarea button select hr a)
#app
.pixel-img
.con-dialog-row (p span input button)
```

### [App]
```
.lab-version-number
```

### [ContextMenu]
```
(*)
.pan-conmenu (ul li button i hr)
    .lab-conmenu-shortcut
```

### [PageLogin]
```
.con-login
    #gra-login-logo
    .pan-login
        .con-login-input
            .inp-login
            .btn-login
    .lab-splash-text
```

### [PageMain]
```
.con-main
    .con-sidebar
        .con-top-buttons
            .btn-aster
                #gra-main-logo
            .btn-add-server
            .btn-account
    .con-channel-edge-separator
```

### [PanelServerList]
```
.con-server-list
```

### [PanelServerView]
```
.con-server-area
    .pan-server-channels
        .con-server-info
            .lab-server-info
            .btn-server-profile
    .pan-server-messages
        .con-message-area
        .con-message-input
            .inp-message
        .con-channel-toggle
            .btn-channel-list
```

### [PanelChannelList]
```
.con-channel-list
```

### [Dialog]
```
.pan-bg-darken
    #gra-dialog-logo
    .pan-dialog
    .lab-dialog-title
    .con-dialog-content
    .con-dialog-buttons
        .btn-dialog-exit
```

### [DialogAccount]
```
#pan-dialog-account
    .gra-account-pfp
    .con-account-pfp
        .gra-account-pfp
        .btn-account-pfp
```

### [DialogAddServer]
```
#pan-dialog-addserver
```

### [DialogChangelog]
```
#pan-dialog-changelog
    .con-changelog-scrollbox
```

### [DialogImage]
```
#pan-dialog-image
    .con-image-img
        .gra-image-img
```

### [DialogKeybinds]
```
#pan-dialog-keybinds
.lab-keybind
```

### [DialogMemberList]
```
#pan-dialog-memberlist
    .con-memberlist-scrollbox
        .con-memberlist-member
            .gra-memberlist-pfp
            .lab-memberlist-displayname
```

### [DialogServerProfile]
```
#pan-dialog-serverprofile
    .con-serverprofile-pfp
        .gra-serverprofile-pfp
        .btn-serverprofile-pfp
```

### [DialogTheme]
```
#pan-dialog-theme
    .btn-theme-file
    .inp-select-lang
```

### [ServerListButton]
```
.con-btn-server
    .btn-server
        .con-sever-name
            .gra-server-icon
            .lab-server-name
        .lab-server-tagline
```

### [ChannelListButton]
```
.btn-channel
```

### [ServerMessage]
```
.con-message
    .gra-message-pfp
    .lab-message-username
    .con-message-body
        .lab-message-username-mobile
    .con-message-image
        .gra-message-image
    .lab-message-date-mobile
    .lab-message-date
```

---
[Aster Web]: ../index
[Component]: ../components/

[App]: ./app
[ContextMenu]: ./contextmenu
[PageLogin]: ./pagelogin
[PageLoading]: ./pageloading
[PageMain]: ./pagemain
[PanelServerList]: ./panelserverlist
[PanelServerView]: ./panelserverview
[PanelChannelList]: ./panelchannellist
[Dialog]: ./dialog
[DialogAccount]: ./dialogaccount
[DialogAddServer]: ./dialogaddserver
[DialogChangelog]: ./dialogchangelog
[DialogImage]: ./dialogimage
[DialogKeybinds]: ./dialogkeybinds
[DialogMemberList]: ./dialogmemberlist
[DialogServerProfile]: ./dialogserverprofile
[DialogTheme]: ./dialogtheme
[ServerListButton]: ./serverlistbutton
[ServerMessage]: ./servermessage
[ChannelListButton]: ./channellistbutton