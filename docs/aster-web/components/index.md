---
title: Components
layout: default
has_toc: false
parent: Aster Web
nav_order: 1
---

# Components in Aster Web
Aster Web is built using [Svelte](https://svelte.dev/) and as such it is comprised of components which are written in `.svelte` files. Below is the hierarchy of all of the Svelte components in Aster Web.

```
App
 ├─ PageLogin
 ├─ PageLoading
 ├─ PageMain
 │   ├─ DialogTheme
 │   ├─ DialogAddServer
 │   ├─ DialogAccount
 │   ├─ PanelServerList
 │   │   └─ ServerListButton
 │   └─ PanelServerView
 │       ├─ DialogServerProfile
 │       ├─ DialogKeybinds
 │       ├─ DialogMemberList
 │       ├─ ServerMessage
 │       ├─ DialogImage
 │       └─ PanelChannelList
 │          └─ ChannelListButton
 ├─ DialogChangelog
 └─ Context Menu
```

Note that there is also the [Dialog] component which is utilised by all of the other `Dialog-` prefixed components.

Below is an overview of all of the components and their functions:

- [App] - Primary container for the web app.
- [ContextMenu] - Context-specific right click menu.
- [PageLogin] - Login page.
- [PageLoading] - Blank page with a loading spinner.
- [PageMain] - The main page and layout of Aster Web.
- [PanelServerList] - Container for list of [ServerListButton]\(s\).
- [PanelServerView] - Container for the chat environment of the selected server.
- [PanelChannelList] - Container for list of [ChannelListButton]\(s\).
- [Dialog] - Base setup for all popups and dialogs within Aster Web.
- [DialogAccount] - Account settings dialog.
- [DialogAddServer] - Add new server dialog.
- [DialogChangelog] - Changelog / patch notes dialog.
- [DialogImage] - Large display for images send in servers.
- [DialogKeybinds] - Help menu / keybinds dialog.
- [DialogMemberList] - List of members in a server.
- [DialogServerProfile] - Server specific profile settings dialog.
- [DialogTheme] - Aster Web theme settings dialog.
- [ServerListButton] - Server button
- [ServerMessage] - Container for a message within a server
- [ChannelListButton] - Channel button

---

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